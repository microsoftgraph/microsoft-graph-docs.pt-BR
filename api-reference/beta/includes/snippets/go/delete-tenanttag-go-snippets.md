---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c89522a4a91f3c820880fdc39119e6359ce6c3b1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411579"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantTagId := "tenantTag-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Delete(nil)


```