---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d592ad050ecaa73daf983fe92746cdc88e7906d9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323891"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().InformationProtection().Policy().Labels().Get()


```