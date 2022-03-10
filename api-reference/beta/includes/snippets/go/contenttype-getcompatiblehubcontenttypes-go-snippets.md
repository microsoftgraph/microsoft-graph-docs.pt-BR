---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b29542de7b5a4d00dfab5255416a2e768aa6579f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411164"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().GetCompatibleHubContentTypes()(site-id, list-id).Get(nil)


```