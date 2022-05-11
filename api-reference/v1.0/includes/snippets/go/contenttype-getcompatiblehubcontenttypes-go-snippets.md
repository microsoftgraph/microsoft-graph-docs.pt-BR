---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4867a8695e3a7a9ec6e3d91385eb3a4e51f8ba85
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316091"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().GetCompatibleHubContentTypes()(site-id, list-id).Get()


```