This file tracks important changes in PRs

geoopt v.0.1.1
==============

New Features
------------
* Add ``geoopt.ismanifold`` utility

Bug Fixes
---------
* Fix typing compatibility with python 3.7+


geoopt v0.1.0
=============

Breaking Changes
----------------
* Better public api, refactored developer api a lot (#40). See the corresponding PR for more details
* Refactored internal design, caused another api change (#77)
* Removed ``t`` argument from everywhere (#76). The argument just scaled tangent vectors but
appeared to be very problematic in maintenance


New Features
------------
* Added ``Sphere`` manifold (#25)
* Added ``SphereSubspaceIntersection``, ``SphereSubspaceComplementIntersection`` manifolds (#29)
* Added expmap implementation (#43)
* Added dist, logmap implementation (#44)
* Added Poincare Ball model (#45)
* Poincare Ball manifold has now new methods (#78)
* Added ``ndim`` argument to ``Euclidean`` manifold
* Added ``Product`` manifold (#109)
* Added ``Scaled`` manifold (#109)
* Unified ``random`` for manifolds (#109) so it can be used in product manifold
* Added ``origin`` for manifolds (#109), it is useful for embeddings

Maintenance
-----------
* Add gitter chat (#31)
* Maintain torch>=1.0.0 only (#39)
* Manifolds are Modules (#49)
* Replace deprecated functions in torch>=1.1.0 (#67)
* Remove PyManOpt from test requirements (#75)
* Add pylint, pydoctest, pydocstyle to travis

Bug Fixes
---------
* Make pickle work with ManifoldTensors (#47)
* Resolve inconsistency with tensor strides and optimizer updates (#71)
