---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13600b62330a518d9b3e8774bf390e2e22e9bd72
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322373"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Delete()


```