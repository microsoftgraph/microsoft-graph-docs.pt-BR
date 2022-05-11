---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12666e8691b307c90867858b3f913e38df801a03
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).AudioRoutingGroups().Get()


```