Reusable definitions for isolating composable contract components.

Attempts to expressly overrides default rules of interpretation that would make the legal effect of a contract component dropped into a larger agreement unpredictable.

***This language is highly experimental. Use at your own risk.***

# Development

The language is provided in Common Form markup.

# Use

Apply to a specific part of a contract as follows:

> Article X. _Payment Terms_.
>
> Section 10.1. _Invoices_. \[...\]
>
> Section 10.2. _Net 30_. \[...\]
>
> Section 10.3. _Disputed Amounts_. \[...\]
>
> Section 10.4. _Late Payment Remedies_. \[...\]
>
> Section 10.5. _Component_. This Article X is a Component.

Or in Common Form markup:

```commonform
\ Payment Terms \

    \ Invoices \ ...

    \ Net 30 \ ...

    \ Disputed Amounts \ ...

    \ Late Payment Remedies \ ...

    \ Component \ {Payment Terms} is a <Component>.
```
