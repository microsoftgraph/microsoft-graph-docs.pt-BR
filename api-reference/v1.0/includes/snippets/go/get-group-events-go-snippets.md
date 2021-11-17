---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 503ef3d2391fba014e329255c4f38b3b5cb5d4b1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993148"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Events().Get(options)


```