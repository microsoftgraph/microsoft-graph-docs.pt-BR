---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: adb76dce79be3f24574702eabc840ea1973dd628
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325478"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
externalItemId := "externalItem-id"
graphClient.External().ConnectionsById(&externalConnectionId).ItemsById(&externalItemId).Delete()


```