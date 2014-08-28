Commerce Deposit
================

# Module setup

Download and enable the module as usual.

# Product types

In order for the deposit system to work properly, we need to specify which
product types are allowed to have a deposit. We do this by utilizing a Boolean
field. We only need to create this field once, then it can be used across each
product type (if we have multiple)

To enable deposits on a particular product type, for example, go to:

1. Go to: Store -> Products -> Product types -> Product -> Manage fields
          (admin/commerce/products/types/product/fields)
2. Add new field (only add once, and instead use "Add existing field" next time)
     Label: Deposit
     Machine name (very important): field_commerce_deposit
     Field type: Boolean
     Widget: Single on/off checkbox
3. Click "Save"
4. Leave the "On value" and "Off value" text fields blank
5. Click "Save field settings"
6. Check the box for "Use field label instead of the 'On Value' as label"
7. Click "Save settings"

# Products

Now that we have a boolean field to indicate which products are allowed to have
a deposit, we need to specify which products will have deposits.

1. Go to: Store -> Products
          (admin/commerce/products)
2. Click "edit" next to a product that is allowed to have a deposit
3. Check the box next to "Deposit"
4. Click "Save Product"
5. Repeat this for each product that can have a deposit

If you have many products that need to be marked, use the Views Bulk Operations
module to save yourself much time.

