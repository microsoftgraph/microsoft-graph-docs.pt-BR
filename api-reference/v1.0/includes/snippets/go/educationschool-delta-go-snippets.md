---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4ce020addbe85b020f1752b90046f9261d6b51f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324228"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Schools().Delta()().Get()


```