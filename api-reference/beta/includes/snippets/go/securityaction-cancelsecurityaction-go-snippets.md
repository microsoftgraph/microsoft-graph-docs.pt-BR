---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e30f3ec75b92b79bc74bceeaca146f3ba060e405
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325025"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

securityActionId := "securityAction-id"
graphClient.Security().SecurityActionsById(&securityActionId).CancelSecurityAction(securityAction-id).Post()


```