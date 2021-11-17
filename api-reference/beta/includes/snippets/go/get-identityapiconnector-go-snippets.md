---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28c779d2323927dfc67b8a7be961f61ae0211f84
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986198"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

identityApiConnectorId := "identityApiConnector-id"
result, err := graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).Get(options)


```