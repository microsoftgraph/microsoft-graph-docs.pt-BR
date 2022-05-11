---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 744c393ba9a618e2ac2bd945b1834e59b91439b6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322351"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().RegisteredDevices().Get()


```