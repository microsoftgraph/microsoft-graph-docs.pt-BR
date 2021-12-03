---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14158a137771523b8dfba6a88eb737a7145b0e5a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286527"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
listItemVersionId := "listItemVersion-id"
graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).VersionsById(&listItemVersionId).RestoreVersion().Post(nil)


```