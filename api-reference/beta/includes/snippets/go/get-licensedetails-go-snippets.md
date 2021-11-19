---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2876b6910598acc841a7815f06caf0023a7c62bc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085952"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().LicenseDetails().Get(options)


```