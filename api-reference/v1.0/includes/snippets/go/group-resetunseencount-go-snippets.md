---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebdbbe65e60493b51c85a334d31265a991ee8c13
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411419"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.GroupsById(&groupId).ResetUnseenCount(group-id).Post(nil)


```