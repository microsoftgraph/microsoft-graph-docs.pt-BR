---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fefd93c9aeb88e2a1b3ffe031b838ec07ba41c20
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094988"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programId := "program-id"
result, err := graphClient.ProgramsById(&programId).Controls().Get(options)


```