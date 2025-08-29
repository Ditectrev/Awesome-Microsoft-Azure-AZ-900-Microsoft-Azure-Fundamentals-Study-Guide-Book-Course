# Availability Sets

## Important Notes from Recording

During the recording, I couldn't see the separately created Availability Set because I was in another resource group. This is a common issue when working with Azure resources across different resource groups.

## Availability Set Requirements

**Critical**: Availability Sets must be added to Virtual Machines during their creation process. It is not possible to add an Availability Set to an existing VM after it has been deployed. This is a fundamental limitation of Azure's architecture.

### Best Practices

- Always plan your availability set strategy before creating VMs
- Create the availability set first, then reference it when creating VMs
- Ensure all VMs that need to be part of the same availability set are created together
- Consider using availability zones as an alternative for newer regions
