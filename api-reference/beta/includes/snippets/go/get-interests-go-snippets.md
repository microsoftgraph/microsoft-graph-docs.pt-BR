---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee2e205055ab3a54ac6913c5d4694011a93d2aee
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019428"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Profile().Interests().Get(options)


```