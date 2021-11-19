---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7d6cd7ed4ea2b363d8ae57b3081b7aa8f5ab38a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093199"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcOverviewTenantId := "cloudPcOverview-tenantId"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcsOverviewById(&cloudPcOverviewTenantId).Get(options)


```