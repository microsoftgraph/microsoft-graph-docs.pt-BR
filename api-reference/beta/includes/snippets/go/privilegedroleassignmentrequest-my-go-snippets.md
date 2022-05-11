---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8446e43b773cdea344981e808adbeaca8e8f62e7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316174"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.PrivilegedRoleAssignmentRequests().My()().Get()


```