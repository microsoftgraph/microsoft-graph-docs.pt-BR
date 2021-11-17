---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13d316ddaca2eed38830796a58db36c0faa8ea26
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016697"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().RegisteredDevices().Get(options)


```