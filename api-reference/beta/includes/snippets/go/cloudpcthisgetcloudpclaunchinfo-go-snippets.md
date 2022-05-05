---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b01e0f7ae356d3e28c6beb35d0762f00c50a0aec
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209323"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPCId := "cloudPC-id"
result, err := graphClient.Me().CloudPCsById(&cloudPCId).GetCloudPcLaunchInfo()(cloudPC-id).Get(nil)


```