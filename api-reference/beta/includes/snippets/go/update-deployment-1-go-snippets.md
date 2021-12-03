---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d32a96698862714de3ddc6c3f9c9ab5f4a81f797
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286778"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deploymentId := "deployment-id"
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Patch(nil)


```