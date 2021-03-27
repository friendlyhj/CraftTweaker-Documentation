# IMutableItemStack

An mutable ItemStack. `withTag` `withAmount` `damageItem` etc. will modify and return the ItemStack itself.

## Importing the package

It might be required for you to import the package if you encounter any issues (like casting an [Array](/AdvancedFunctions/Arrays_and_Loops/)), so better be safe than sorry and add the import.  
`import crafttweaker.item.IMutableItemStack;`

## Getting the Instance

Use IItemStack's  `mutable()` method.

## Extending the IItemStack

IMutableItemStack extends [IItemStack](/Vanilla/Items/IItemStack/) and are able to call all of its methods/getters/setters as well.

## ZenMethods

### Quantity

Besides `withAmount`, you can easily call these methods below to change the count of item.

| ZenMethod       | Parameter Type | Description                                         |
|-----------------|----------------|-----------------------------------------------------|
| grow(count)     | int            | Increases the stack's count by the `count` provided |
| shrink(count)   | int            | Decreases the stack's count by the `count` provided |

### Copying

`IItemStack copy();`

The copy method will returns a new immutable stack with the same properties. If you are certain that the stack shouldn't be changed anymore and want to avoid unexpected item changes, you will need to use the method.