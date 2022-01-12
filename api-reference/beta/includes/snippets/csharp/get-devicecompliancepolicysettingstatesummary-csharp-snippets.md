---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6f5d9e820a5d4971197555baa93510cd3ef2f5540bf33857ad74eef982e70dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157608"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.TenantRelationships.ManagedTenants.DeviceCompliancePolicySettingStateSummarys["{UNKNOWN-id}"]
    .Request()
    .GetAsync();

```