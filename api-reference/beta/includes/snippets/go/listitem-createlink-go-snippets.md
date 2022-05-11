---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 576311c0734480111816921d42039d82cf203497
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325147"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
type := "embed"
requestBody.SetType(&type)
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).CreateLink(site-id, list-id, listItem-id).Post(requestBody)


```