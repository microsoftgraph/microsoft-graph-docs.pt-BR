---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27356e87a68f29040070fbaa72d64c83b6dd6bca
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322997"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().Anniversaries().Get()


```