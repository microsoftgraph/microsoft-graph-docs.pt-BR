---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1af907c0443a8990f345989caccfd6470ce06146
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287336"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().OwnedDevices().Get(nil)


```