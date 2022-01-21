---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3d5a9b2159b4faf0a58cc4daf042ecc8972e30a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111056"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Me().Assignments().Get(nil)


```