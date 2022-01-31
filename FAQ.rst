
Q: What if a package has no repository or is proprietary?

- A: Use a "generic" purl and a download URL or homepage URL qualifier.

Q: What if I want to provide file details?

- A: Use a purl with a subpath.

Q: What if I want to provide checksums?

- A: Use a purl with checksum qualifier(s).

Q: Where do I document my own code?

- A: As entries in the packages list. The first item(s)
  would typically describe your own software.

Q: What about vulnerabilities?

- A: If we want a kissbom to also contains vulnerability
  information for packages, we can add a field that would list
  vulnerability ids for this SBoM entry. 
  
Q: Does the kissbom-spec meet NTIA standards for Baseline Attributes?

- A: Based on the discussion in https://github.com/kissbom/kissbom-spec/issues/1
  it likely does
