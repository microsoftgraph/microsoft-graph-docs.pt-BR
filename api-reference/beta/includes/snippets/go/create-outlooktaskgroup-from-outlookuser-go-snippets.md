---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf7a23c08652f3224896ae4f7f2ea399f449409c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324710"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskGroup()
name := "Leisure tasks"
requestBody.SetName(&name)
result, err := graphClient.Me().Outlook().TaskGroups().Post(requestBody)


```