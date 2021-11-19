---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7f95db39b619f5a6d2d78e3eb894b4d4f24625d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104122"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Relations().Get(options)


```