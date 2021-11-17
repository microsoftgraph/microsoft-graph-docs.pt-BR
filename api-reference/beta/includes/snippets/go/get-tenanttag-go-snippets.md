---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bdcde62cfb5e36d56459e2556e58604a9e4cea7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022032"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

tenantTagId := "tenantTag-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Get(options)


```