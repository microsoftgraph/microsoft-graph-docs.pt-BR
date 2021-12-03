---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11f1bb8f0a05a929087a5e3f815f7fd111274fd7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287406"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).RejectedSenders().Get(nil)


```