---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8d307984a85af1feff75ccc68dc92ea0463ac69
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287148"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).MemberOf().Get(nil)


```