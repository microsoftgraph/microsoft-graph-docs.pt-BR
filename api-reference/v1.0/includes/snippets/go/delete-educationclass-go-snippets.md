---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7aad98e00d97f09172785a3929fadd6ee221ddc5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285772"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).Delete(nil)


```