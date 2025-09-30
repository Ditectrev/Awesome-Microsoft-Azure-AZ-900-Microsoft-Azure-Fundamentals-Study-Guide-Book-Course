# How to Delete Storage Account with Resource Lock

## Recording Note

During recording I haven't deleted storage account because it had a resource lock. Here is an instruction how to do it. I've done it offline.

## Step-by-Step Instructions

### Method 1: Using Azure Portal

1. **Navigate to the Resource Group**
   - Go to Azure Portal
   - Find your resource group that contains the storage account

2. **Remove the Resource Lock**
   - In the resource group blade, go to **Settings** → **Locks**
   - Find the existing lock
   - Click on the lock and select **Delete**
   - Confirm the deletion of the lock

3. **Delete the Storage Account**
   - Navigate to the storage account within the resource group
   - Go to the storage account **Overview** page
   - Click **Delete** at the top of the page
   - Type the storage account name to confirm deletion
   - Click **Delete** to permanently remove the storage account

## Important Notes

- **Resource locks prevent accidental deletion** - they must be removed before deleting the resource
- **Lock types**:
  - `CanNotDelete`: Allows read and modify operations but prevents deletion
  - `ReadOnly`: Allows only read operations
- **Permissions required**: You need `Owner` or `User Access Administrator` role to manage locks
- **Double-check before deletion**: Storage account deletion is permanent and cannot be undone
