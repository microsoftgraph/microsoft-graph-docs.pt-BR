---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b15c166c90a54627ad646f91e1d85887f7cac1b3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322197"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
graphClient.TermStore().SetsById(&setId).Delete()


```