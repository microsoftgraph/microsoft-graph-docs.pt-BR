---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 123598d7b8610c0f3d7ccd9a5b7185ff4e509a01
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137536"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Schools().Delta()().Get(nil)


```