---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1653e3e35a4cda2ebd5fd0e2ce541383048a9d94
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
graphClient.GroupsById(&groupId).SubscribeByMail().Post(options)


```