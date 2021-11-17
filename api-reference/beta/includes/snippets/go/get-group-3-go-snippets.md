---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1df77dccc8868bdb0eb496d2b71e7eea994cedfe
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017489"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
result, err := graphClient.TermStore().GroupsById(&groupId).Get(options)


```