---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf59350612168fa53c3d525abbc0cf85a2a59f70
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324061"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Outlook().MasterCategories().Get()


```