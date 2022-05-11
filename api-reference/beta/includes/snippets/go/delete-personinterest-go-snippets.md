---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b33cb324c109cfcb990aae9ca121fe66baf89152
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323109"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personInterestId := "personInterest-id"
graphClient.Me().Profile().InterestsById(&personInterestId).Delete()


```