---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0391bc38c8517ee7a65a7305ae59dc54d8d9ea28
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336169"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var crossTenantAccessPolicyConfigurationPartner = new CrossTenantAccessPolicyConfigurationPartner
{
    InboundTrust = new CrossTenantAccessPolicyInboundTrust
    {
        IsMfaAccepted = true,
        IsCompliantDeviceAccepted = true,
        IsHybridAzureADJoinedDeviceAccepted = true
    }
};

await graphClient.Policies.CrossTenantAccessPolicy.Partners["{crossTenantAccessPolicyConfigurationPartner-id}"]
    .Request()
    .UpdateAsync(crossTenantAccessPolicyConfigurationPartner);

```