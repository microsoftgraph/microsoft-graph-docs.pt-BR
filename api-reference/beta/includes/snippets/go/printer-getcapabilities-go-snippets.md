---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 293d0fbf25ec69dfddd238b98004fd8f13379741
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129580"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).GetCapabilities()().Get(nil)


```