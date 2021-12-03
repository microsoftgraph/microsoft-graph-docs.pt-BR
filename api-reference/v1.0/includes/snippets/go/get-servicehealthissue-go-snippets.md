---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a24b0b530caee181bcc82c41c0e15968f97ac92a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287122"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceHealthIssueId := "serviceHealthIssue-id"
result, err := graphClient.Admin().ServiceAnnouncement().IssuesById(&serviceHealthIssueId).Get(nil)


```