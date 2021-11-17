---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8bf4bcaec8d8edc859882ef28b539ffb31e6d65a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002929"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

conditionalAccessPolicyCoverageId := "conditionalAccessPolicyCoverage-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ConditionalAccessPolicyCoveragesById(&conditionalAccessPolicyCoverageId).Get(options)


```