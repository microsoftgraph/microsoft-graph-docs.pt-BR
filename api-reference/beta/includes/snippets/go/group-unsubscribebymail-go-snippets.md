---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5bae5574396bb90264ddaabbcb297b97b3262cea
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285754"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.GroupsById(&groupId).UnsubscribeByMail().Post(nil)


```