---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 077889d770e1754df0ad9e71a79a8e321dd8ce18
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123314"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Outlook().SupportedLanguages()().Get(nil)


```