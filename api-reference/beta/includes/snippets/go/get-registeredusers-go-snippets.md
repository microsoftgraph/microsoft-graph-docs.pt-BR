---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3e5417f96ca00115506807692a659e8ad46f4ae
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286092"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).RegisteredUsers().Get(nil)


```