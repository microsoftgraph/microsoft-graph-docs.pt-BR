---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9857a38cba9ebe490d870be1ecc2629fe489469f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025398"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).GroupLifecyclePolicies().Get(options)


```