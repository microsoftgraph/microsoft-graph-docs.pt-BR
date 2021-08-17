---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4774bc424a3486e68d79022969f72c6e68eefc0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mobilityManagementPolicy = new MobilityManagementPolicy
{
    ComplianceUrl = "https://portal.mg.contoso.com/?portalAction=Compliance",
    DiscoveryUrl = "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc",
    TermsOfUseUrl = "https://portal.mg.contoso.com/TermsofUse.aspx"
};

await graphClient.Policies.MobileAppManagementPolicies["{mobilityManagementPolicy-id}"]
    .Request()
    .UpdateAsync(mobilityManagementPolicy);

```