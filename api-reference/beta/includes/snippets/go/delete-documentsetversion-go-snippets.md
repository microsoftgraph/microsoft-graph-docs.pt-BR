---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69bc969bad32f2d6950612e9f188880c174ee45e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325245"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
documentSetVersionId := "documentSetVersion-id"
graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).DocumentSetVersionsById(&documentSetVersionId).Delete()


```