---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c23be89e0cbca7f2118eee8613006d92ed99f138
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322678"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookmarkId := "bookmark-id"
result, err := graphClient.Search().BookmarksById(&bookmarkId).Get()


```