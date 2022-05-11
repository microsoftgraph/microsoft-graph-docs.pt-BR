---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 750864b03bd49060a436f1d81cd0ef1f93c59986
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322366"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
riskyUserHistoryItemId := "riskyUserHistoryItem-id"
result, err := graphClient.IdentityProtection().RiskyUsersById(&riskyUserId).HistoryById(&riskyUserHistoryItemId).Get()


```