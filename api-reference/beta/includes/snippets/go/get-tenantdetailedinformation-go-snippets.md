---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6c55687f3dd4c4c2dc68893270c30c35f337b5c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286334"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantDetailedInformationId := "tenantDetailedInformation-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsDetailedInformationById(&tenantDetailedInformationId).Get(nil)


```