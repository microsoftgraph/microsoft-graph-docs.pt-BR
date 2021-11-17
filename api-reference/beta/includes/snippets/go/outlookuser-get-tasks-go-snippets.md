---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44df4717d74e017ee2437cf80de1fc6936b0257e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029970"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Outlook().Tasks().Get(options)


```