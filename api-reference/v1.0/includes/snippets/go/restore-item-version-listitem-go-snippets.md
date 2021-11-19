---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f40f0aacb80948c06d743658696d3e3315e92092
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081570"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
listItemVersionId := "listItemVersion-id"
graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).VersionsById(&listItemVersionId).RestoreVersion().Post(options)


```