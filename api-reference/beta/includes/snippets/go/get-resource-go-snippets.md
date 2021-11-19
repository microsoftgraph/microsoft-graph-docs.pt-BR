---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04c6049fe504e8363d75e5404fbb82f8817457df
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090460"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onenoteResourceId := "onenoteResource-id"
graphClient.Me().Onenote().ResourcesById(&onenoteResourceId).Content().Get(options)


```