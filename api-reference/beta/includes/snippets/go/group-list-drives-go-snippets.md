---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53659f5357d4b8dec2cace8a23f8019b2c612d87
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286052"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Drives().Get(nil)


```