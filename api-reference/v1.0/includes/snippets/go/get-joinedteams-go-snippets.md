---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7d4db48e715dfd7369bd2185f18dbbc18e06a0a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287116"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().JoinedTeams().Get(nil)


```