---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f25936bffb3129bfb087a1e28df8e92df7ea9ae5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009858"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
graphClient.UsersById(&userId).Delete(options)


```