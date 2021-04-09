# e4s-policies
Versioned archive of E4S policies

Version 0.01 of the e4s policies yaml format uses the following structure:
```
#The version of the e4s policies contained in this file
e4s_policy_version: 1
#The version of the format used by this file
e4s_policy_format_version: 0.01
#A list of sub-groups of policies. As of this writing only the 'Official' policy group is relevant to E4S community compliance. Others are included for reference.
policy_groups:
  #An object defining a group of policies
  - Official:
      #The title or short description associated with these policies in the official policy document.
      title: The policies below are criteria for E4S membership
      #The 'preamble' or detailed description associated with these policies in the official policy document
      preamble: >
        To qualify for E4S
        membership, a package must demonstrate compatibility with each of these
        policies. Under special circumstances, a package may be granted an
        exception to a policy.
      #The policy type tag used in conjunction with the id when listing individual policies in the official policy document
      Tag: P
      #The list of individual policies.
      policies:
        #The policy id, equivalent to its order in its group in the official policy document
        - id: 1
          #The name of the policy
          name: Spack-based Build and Installation
          #The full description of the policy
          description: >
            Each E4S member package supports a scriptable Spack build and
            production-quality installation in a way that is compatible with
            other E4S member packages in the same environment. When E4S build,
            test, or installation issues arise, there is an expectation that
            teams will collaboratively resolve those is
```
