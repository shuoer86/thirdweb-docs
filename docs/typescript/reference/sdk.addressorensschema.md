---
slug: /reference/sdk.addressorensschema
title: AddressOrEnsSchema variable
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# AddressOrEnsSchema variable

**Signature:**

```typescript
AddressOrEnsSchema: z.ZodUnion<
  [
    z.ZodType<string, z.ZodTypeDef, string>,
    z.ZodType<`0x${string}`, z.ZodTypeDef, `${string}.eth` | `${string}.cb.id`>,
  ]
>;
```