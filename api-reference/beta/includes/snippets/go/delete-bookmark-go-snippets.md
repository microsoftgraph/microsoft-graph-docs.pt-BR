---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d69a31205fc2420f2b5a506c8008d86aa15a509e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338430"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookmarkId := "bookmark-id"
graphClient.Search().BookmarksById(&bookmarkId).Delete(nil)


```