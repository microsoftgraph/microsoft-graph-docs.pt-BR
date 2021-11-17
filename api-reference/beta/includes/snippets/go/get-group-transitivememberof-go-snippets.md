---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6dbe820449311ef555edf4ba6e55adfcc809ab0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978187"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).TransitiveMemberOf().Get(options)


```