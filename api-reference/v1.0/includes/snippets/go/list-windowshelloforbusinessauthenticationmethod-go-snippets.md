---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99afcdf39abdd677af106025bfff1048af5dc8e2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323147"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().WindowsHelloForBusinessMethods().Get()


```