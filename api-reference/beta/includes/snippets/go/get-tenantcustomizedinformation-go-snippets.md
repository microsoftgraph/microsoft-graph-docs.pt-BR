---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f77408d959e189684d6be14e3777e5462690eb83
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323888"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantCustomizedInformationId := "tenantCustomizedInformation-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsCustomizedInformationById(&tenantCustomizedInformationId).Get()


```