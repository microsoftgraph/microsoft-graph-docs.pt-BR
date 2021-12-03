---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68a3403164c4a5d3cb7c8399914cc47cfedef1c7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286341"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).AppRoleAssignments().Get(nil)


```