---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b273300d1f0ba44dd372822e9501ae4820c20839
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322194"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Todo().Lists().Get()


```