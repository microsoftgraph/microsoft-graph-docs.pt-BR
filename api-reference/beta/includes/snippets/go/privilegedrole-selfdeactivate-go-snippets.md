---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ade70f57a9a9759cf1acadfc02e6fab54bd7fff3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315228"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleId := "privilegedRole-id"
result, err := graphClient.PrivilegedRolesById(&privilegedRoleId).SelfDeactivate(privilegedRole-id).Post()


```