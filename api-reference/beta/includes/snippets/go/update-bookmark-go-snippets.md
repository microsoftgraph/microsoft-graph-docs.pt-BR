---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3132daf0b79efeda7746c27a381126011650b140
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324575"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookmark()
description := "Book a fancy vacation in Tuscany or browse museums in Florence."
requestBody.SetDescription(&description)
bookmarkId := "bookmark-id"
graphClient.Search().BookmarksById(&bookmarkId).Patch(requestBody)


```