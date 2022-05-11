---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4ab141bdf737edd74b06a01ba5313c83ed141c1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324024"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Classes().Delta()().Get()


```