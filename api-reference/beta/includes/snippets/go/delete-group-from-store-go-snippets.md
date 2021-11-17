---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98cce18219e548986bb268631ee086aba98d33ce
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017468"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
graphClient.TermStore().GroupsById(&groupId).Delete(options)


```