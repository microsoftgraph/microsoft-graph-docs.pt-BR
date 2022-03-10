---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f68e02776956442dcf159f99d46c1615de214485
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411420"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.GroupsById(&groupId).RemoveFavorite(group-id).Post(nil)


```