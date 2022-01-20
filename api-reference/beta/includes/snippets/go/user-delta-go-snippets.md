---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1579ce0a18ecb2dbb27ce0c440202b6d1065116e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Users().Delta()().Get(nil)


```