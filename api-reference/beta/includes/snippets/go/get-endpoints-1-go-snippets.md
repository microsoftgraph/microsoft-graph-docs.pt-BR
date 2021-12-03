---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c76d8b7d2d1668b8fe3b7d00e179f2bf1c51c1de
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285756"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Endpoints().Get(nil)


```