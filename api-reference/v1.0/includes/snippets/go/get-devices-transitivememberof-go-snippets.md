---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 045a9a1de48a5fe47c37c266d2b0a9976b8612c1
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287478"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).TransitiveMemberOf().Get(nil)


```