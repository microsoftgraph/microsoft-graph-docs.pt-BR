---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd30ba39c1b5e0b94874bae0bc0fcd1d6f9469a5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989606"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).AllowedUsers().Get(options)


```