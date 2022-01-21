---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 490d232c4c045683c65e748bd83c83ce288a7324
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137605"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Groups().Delta()().Get(nil)


```