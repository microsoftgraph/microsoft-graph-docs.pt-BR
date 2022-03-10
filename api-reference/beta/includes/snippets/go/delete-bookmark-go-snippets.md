---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfffee49305ca8b9f5d69c53597f361e2733b870
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411520"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookmarkId := "bookmark-id"
result, err := graphClient.Search().BookmarksById(&bookmarkId).Delete(nil)


```