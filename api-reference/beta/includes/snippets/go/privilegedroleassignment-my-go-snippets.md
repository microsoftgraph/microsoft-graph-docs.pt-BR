---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7876731c56a6c7eb0881fb9cc5e024b5e3d29a73
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314247"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.PrivilegedRoleAssignments().My()().Get()


```