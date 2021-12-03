---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58ef1a30ad95b856c8a9ff9291483042d39bc62a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286440"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantTagId := "tenantTag-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Get(nil)


```