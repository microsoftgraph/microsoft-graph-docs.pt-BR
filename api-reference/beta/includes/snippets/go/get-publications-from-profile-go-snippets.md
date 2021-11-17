---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2b6c3e7186f340e89d0573dede1de9adad13a1c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019358"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Profile().Publications().Get(options)


```