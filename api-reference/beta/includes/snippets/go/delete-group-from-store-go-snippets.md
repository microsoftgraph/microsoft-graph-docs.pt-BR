---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f31dc89944c04a754f6ec4ec3ee3aa86e68fd675
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084175"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.TermStore().GroupsById(&groupId).Delete(options)


```