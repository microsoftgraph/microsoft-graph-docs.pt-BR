---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ee5fcc66f38624fc1ecac586a3474cd665a9e32
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944911"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment
{
    IsOptional = false,
    RequiresVerification = false,
    UserInputType = IdentityUserFlowAttributeInputType.TextBox,
    DisplayName = "Shoe size",
    UserAttributeValues = new List<UserAttributeValuesItem>()
    {
    },
    UserAttribute = new IdentityUserFlowAttribute
    {
        Id = "extension_guid_shoeSize"
    }
};

await graphClient.Identity.B2cUserFlows["B2C_1_Consumer"].UserAttributeAssignments
    .Request()
    .AddAsync(identityUserFlowAttributeAssignment);

```