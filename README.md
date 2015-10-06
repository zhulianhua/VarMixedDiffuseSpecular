# VarMixedDiffuseSpecular

In the standard `dsmcFoam` solver (OF 2.4.0), the `wallInteractionModel` is a global parameter.
Which means each part of the wall uses the same wall interaction model. The diffusive fraction is the same everywhere.

In this project, a new wall interaction model is defined, called "`VarMixedDiffuseSpecular`".
It allow us to use  a diffusive fraction variable associate with each wall patch.

To specify the diffusive fraction parameters, we use the `alphaFixedValued` type boundary type for the wall temperature boundary condition.
