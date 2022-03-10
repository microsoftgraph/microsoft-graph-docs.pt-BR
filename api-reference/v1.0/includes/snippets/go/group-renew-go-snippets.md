---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad0f0da7374e567ddb8a7dc7c003c3f45d690351
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410980"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.GroupsById(&groupId).Renew(group-id).Post(nil)


```