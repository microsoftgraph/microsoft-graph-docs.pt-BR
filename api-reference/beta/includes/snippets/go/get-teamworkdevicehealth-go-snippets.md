---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f63b20514cf395ed9958b8db8dc39c05c8db0d8a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349015"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamworkDeviceId := "teamworkDevice-id"
result, err := graphClient.Teamwork().DevicesById(&teamworkDeviceId).Health().Get(nil)


```