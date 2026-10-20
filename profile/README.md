# rtnx-methods

Open implementations of published methods in rock mechanics and surface
blasting, with test vectors taken from worked examples in the literature.

Maintained by [RockTech NeXus](https://rocktechnexus.com). These are the same
method implementations used in Rocklytics and mineraX.

## Why this is open

Our products claim that every result shows its method, units, assumptions and
warnings. That claim is not credible if the implementation of the method is
hidden. The equations are published and well known. The work worth checking is
whether they are implemented correctly, against which source, and within which
validity limits.

So the methods are open, and the test vectors that prove them are open too.

## Scope and limitations

This library implements published methods for preliminary assessment and
screening. It is not a substitute for site investigation, monitoring,
project-specific numerical modelling, detailed design, statutory compliance,
independent checking, or professional engineering judgement.

Every method carries stated validity limits. Results obtained outside those
limits are not meaningful. Where we could not trace a coefficient or chart
value to a published source, it is labelled as engineering judgement or
omitted, and the validation register records which.

The user is responsible for deciding whether a method applies to their ground
conditions and for the engineering decisions taken on the basis of any result.

## Methods

| Method | Domain | Status |
| --- | --- | --- |
| RQD, from core run and from volumetric joint count | Rock mass | planned |
| RMR, Bieniawski | Rock mass classification | planned |
| Q system, Barton | Rock mass classification | planned |
| Hoek-Brown parameters, mb, s, a | Rock strength | planned |
| Burden and spacing | Blast design | planned |
| Kuz-Ram | Fragmentation | planned |
| Rosin-Rammler | Fragmentation | planned |

Status is honest. Nothing is marked done until it has test vectors from a
published worked example and a recorded source.

## Test vectors

Each method ships with fixtures taken from worked examples in the literature:
inputs, expected output, tolerance, full citation with DOI where one exists,
and the validity limits that applied in the source.

These run in CI on every commit. A method whose published example does not
reproduce is a failing build, in public.

## Citing

If you use this library in published work, please cite it. See `CITATION.cff`,
or use the "Cite this repository" button on the repository page.

## License

Apache-2.0. See `LICENSE`.
