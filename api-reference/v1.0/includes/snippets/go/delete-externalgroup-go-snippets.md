---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5378b42ce029f27e71b79851ec2d774aa7930c4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324757"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).Delete()


```