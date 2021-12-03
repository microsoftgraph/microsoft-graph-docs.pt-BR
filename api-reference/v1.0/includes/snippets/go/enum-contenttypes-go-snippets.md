---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ce341c9be67051b4e0346abeb5a879971a94bc3
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286515"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().Get(nil)


```