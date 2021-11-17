---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5bac7278ee5a9f29fa4f0cabda5dfb6051589548
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020038"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Get(options)


```