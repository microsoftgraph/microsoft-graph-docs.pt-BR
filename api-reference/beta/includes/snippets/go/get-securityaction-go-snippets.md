---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc124e6f08809062f49c693c58429a230371b118
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286893"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

securityActionId := "securityAction-id"
result, err := graphClient.Security().SecurityActionsById(&securityActionId).Get(nil)


```