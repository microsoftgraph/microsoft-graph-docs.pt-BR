---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19553c5a5ea04e1b7657d693e18b8dad8721f18c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411028"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcOnPremisesConnectionId := "cloudPcOnPremisesConnection-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).Delete(nil)


```