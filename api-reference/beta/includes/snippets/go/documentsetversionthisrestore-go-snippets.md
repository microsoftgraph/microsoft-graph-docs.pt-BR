---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2a74831e53283c61c6d4586edbc109a5487ea39
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325244"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
documentSetVersionId := "documentSetVersion-id"
graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).DocumentSetVersionsById(&documentSetVersionId).Restore(site-id, list-id, listItem-id, documentSetVersion-id).Post()


```