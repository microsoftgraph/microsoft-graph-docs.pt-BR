---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1ec85adcf8b409541553b1eaf9578a92de6e703
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287021"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().DirectReports().Get(nil)


```