---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6ee5c2b9b5feb60019f483920b5c46a6e778d7f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098200"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().Certifications().Get(options)


```