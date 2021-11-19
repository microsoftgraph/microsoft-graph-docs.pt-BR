---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d70768484d93dc8727977f2145a4f92125255299
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097663"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
reason := "reason-value"
requestBody.SetReason(&reason)
ticketNumber := "ticketNumber-value"
requestBody.SetTicketNumber(&ticketNumber)
ticketSystem := "ticketSystem-value"
requestBody.SetTicketSystem(&ticketSystem)
options := &msgraphsdk.MakePermanentRequestBuilderPostOptions{
    Body: requestBody,
}
privilegedRoleAssignmentId := "privilegedRoleAssignment-id"
result, err := graphClient.PrivilegedRoleAssignmentsById(&privilegedRoleAssignmentId).MakePermanent().Post(options)


```