---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 172b9cddc7f235b83372f3993178e5a76b51ea18
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287469"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Owners().Get(nil)


```