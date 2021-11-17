---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27d5af45c59007fc141ce562e7b645d2f3bff96f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033470"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().InvalidateAllRefreshTokens().Post(options)


```