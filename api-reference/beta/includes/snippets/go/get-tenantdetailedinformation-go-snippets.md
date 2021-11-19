---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbcaaccb0ba0964ae40f673c4beeb2e5b345b810
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090976"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantDetailedInformationId := "tenantDetailedInformation-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsDetailedInformationById(&tenantDetailedInformationId).Get(options)


```