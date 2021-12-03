---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49fabdc38eb78bfc07a873fbd3e092ffa74dc499
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
graphClient.DevicesById(&deviceId).Delete(nil)


```