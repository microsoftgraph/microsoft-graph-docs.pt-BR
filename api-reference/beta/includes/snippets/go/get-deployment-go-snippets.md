---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0fe9adb9bd719a4ccc551b51b383041188d55fc2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016592"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

deploymentId := "deployment-id"
result, err := graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Get(options)


```