---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61f1beb3e42f950b858f5ac1903f72175d65a251
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002271"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
result, err := graphClient.UsersById(&userId).Settings().ShiftPreferences().Get(options)


```