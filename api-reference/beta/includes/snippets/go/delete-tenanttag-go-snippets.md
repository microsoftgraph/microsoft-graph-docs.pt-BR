---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73d142747c7cd4cb96943de582ea569c001914fe
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019785"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

tenantTagId := "tenantTag-id"
graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Delete(options)


```