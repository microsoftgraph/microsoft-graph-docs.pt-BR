---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25e47a1f37bf19616097089cf7e1c5a2e179b9e5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098628"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTask()
subject := "Shop for dinner"
requestBody.SetSubject(&subject)
startDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartDateTime(startDateTime)
dateTime := "2016-04-23T18:00:00"
startDateTime.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
startDateTime.SetTimeZone(&timeZone)
dueDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetDueDateTime(dueDateTime)
dateTime := "2016-04-25T13:00:00"
dueDateTime.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
dueDateTime.SetTimeZone(&timeZone)
options := &msgraphsdk.TasksRequestBuilderPostOptions{
    Body: requestBody,
}
outlookTaskFolderId := "outlookTaskFolder-id"
result, err := graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Tasks().Post(options)


```