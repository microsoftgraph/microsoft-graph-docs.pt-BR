---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a16e7ff89cb89e0f0e51d1a1af4906fb6bbe522d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323140"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().PhoneMethods().Get()


```