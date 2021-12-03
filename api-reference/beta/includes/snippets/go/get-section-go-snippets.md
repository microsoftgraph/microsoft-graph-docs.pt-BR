---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7528ecfc8b324acf0e130e15e7b58a52f87bbf69
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286536"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onenoteSectionId := "onenoteSection-id"
result, err := graphClient.Me().Onenote().SectionsById(&onenoteSectionId).Get(nil)


```