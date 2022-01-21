---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1620315002474ddd4b1d6ae85c271d2e8bb098d3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deviceCompliancePolicySettingStateSummaries = await graphClient.TenantRelationships.ManagedTenants.DeviceCompliancePolicySettingStateSummaries
    .Request()
    .GetAsync();

```