---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf4e9c616a5d30429ed2da2b689bf98432992258
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322187"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().MailFolders().Get()


```