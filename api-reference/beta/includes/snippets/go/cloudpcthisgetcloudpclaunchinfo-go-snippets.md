---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5799c7c17ee4017380a5aaa7215d69aaa23deec
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323571"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPCId := "cloudPC-id"
result, err := graphClient.Me().CloudPCsById(&cloudPCId).GetCloudPcLaunchInfo()(cloudPC-id).Get()


```