---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9435fd816f5213d37b7e23d2bc6e1e5fdfd91d0a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410538"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).Delete(nil)


```