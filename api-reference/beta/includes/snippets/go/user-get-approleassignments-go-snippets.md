---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5ca14a542c768819c50538627184c2334643a50
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091908"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).AppRoleAssignments().Get(options)


```