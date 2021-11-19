---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82cac5e63bf6c64f1126ca9137f569e005bd861e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103460"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Outlook().MasterCategories().Get(options)


```