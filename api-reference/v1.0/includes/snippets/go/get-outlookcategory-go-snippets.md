---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b298ee075893b2eb2ad998ade633f210b88a9ec4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103975"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

outlookCategoryId := "outlookCategory-id"
result, err := graphClient.Me().Outlook().MasterCategoriesById(&outlookCategoryId).Get(options)


```