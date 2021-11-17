---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 720a0445b767f506b494ce842a94c932ea2559bf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030027"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcOverviewTenantId := "cloudPcOverview-tenantId"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcsOverviewById(&cloudPcOverviewTenantId).Get(options)


```