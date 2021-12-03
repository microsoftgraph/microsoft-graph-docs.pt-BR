---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 120e727bc7bce2f5ddf27ad96b34aba21840b218
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287366"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).Delete(nil)


```