---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66ac0e3df35bdc1e9fb7074688030d0a99b22f97
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Activities().Recent()().Get()


```