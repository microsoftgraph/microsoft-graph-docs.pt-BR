---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88eaa154a2bd3a64a6746104abb5e8d1ea48ce75
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325024"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceHealthIssueId := "serviceHealthIssue-id"
result, err := graphClient.Admin().ServiceAnnouncement().IssuesById(&serviceHealthIssueId).IncidentReport()(serviceHealthIssue-id).Get()


```