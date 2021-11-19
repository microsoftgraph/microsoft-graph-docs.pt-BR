---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4fe71e7e13507cd0beb56ab3079c26201a738ab2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082088"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
eventId := "event-id"
result, err := graphClient.GroupsById(&groupId).EventsById(&eventId).Get(options)


```