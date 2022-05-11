---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb8babaf74c3b008a60ead2bbc79170485b6ef99
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325603"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

presenceId := "presence-id"
result, err := graphClient.Communications().PresencesById(&presenceId).Get()


```