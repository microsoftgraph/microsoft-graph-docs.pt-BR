---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 126e5b2442e79be08abd4356e280371fe7f79727
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095768"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

conditionalAccessPolicyCoverageId := "conditionalAccessPolicyCoverage-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ConditionalAccessPolicyCoveragesById(&conditionalAccessPolicyCoverageId).Get(options)


```