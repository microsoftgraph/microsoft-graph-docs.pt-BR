---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6be0b52d86cfe5d589692929b34ab045680ece8
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411010"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onenoteResourceId := "onenoteResource-id"
result, err := graphClient.Me().Onenote().ResourcesById(&onenoteResourceId).Content().Get(nil)


```