---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bf25387028dc8c1568ace63575675ad68f958e4258d00b2b9f5a42d6f47658f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100545"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = new ConditionalAccessPolicy
{
    DisplayName = "Require MFA to EXO from non-complaint devices.",
    State = ConditionalAccessPolicyState.Enabled,
    Conditions = new ConditionalAccessConditionSet
    {
        Applications = new ConditionalAccessApplications
        {
            IncludeApplications = new List<String>()
            {
                "00000002-0000-0ff1-ce00-000000000000"
            }
        },
        Users = new ConditionalAccessUsers
        {
            IncludeGroups = new List<String>()
            {
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            }
        },
        Devices = new ConditionalAccessDevices
        {
            IncludeDevices = new List<String>()
            {
                "All"
            },
            ExcludeDevices = new List<String>()
            {
                "Compliant"
            }
        }
    },
    GrantControls = new ConditionalAccessGrantControls
    {
        Operator = "OR",
        BuiltInControls = new List<ConditionalAccessGrantControl>()
        {
            ConditionalAccessGrantControl.Mfa
        }
    }
};

await graphClient.Identity.ConditionalAccess.Policies
    .Request()
    .AddAsync(conditionalAccessPolicy);

```