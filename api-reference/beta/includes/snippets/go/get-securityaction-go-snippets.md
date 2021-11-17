---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 251027f8c8b85874f243e774516b163fa0b7fe5f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

securityActionId := "securityAction-id"
result, err := graphClient.Security().SecurityActionsById(&securityActionId).Get(options)


```