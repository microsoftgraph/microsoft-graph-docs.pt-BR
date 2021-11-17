---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee9582a6541b60b4894e5e99b750a1988dbda7dc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009348"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Settings().ItemInsights().Get(options)


```