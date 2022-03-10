---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8635ab6beae57fd65cd3552f4cef8fea3aaba477
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411418"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.GroupsById(&groupId).SubscribeByMail(group-id).Post(nil)


```