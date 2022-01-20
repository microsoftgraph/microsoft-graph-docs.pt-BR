---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92cc614f7f85e72afd4ee08d0dbb5a79fbf125f8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137537"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DeviceManagement().VirtualEndpoint().DeviceImages().GetSourceImages()().Get(nil)


```