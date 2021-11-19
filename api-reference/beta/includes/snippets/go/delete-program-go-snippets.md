---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4488278e1dd08ea87cbd43a349c3214d70a47e9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programId := "program-id"
graphClient.ProgramsById(&programId).Delete(options)


```