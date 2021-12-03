---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6188b54216e3eda451a151b79b1090a9a1f1aef1
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personAwardId := "personAward-id"
result, err := graphClient.Me().Profile().AwardsById(&personAwardId).Get(nil)


```