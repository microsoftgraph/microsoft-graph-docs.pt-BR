---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da78175ad1b7d6f3dff60b021877922fdf5fd81b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984454"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

outlookCategoryId := "outlookCategory-id"
result, err := graphClient.Me().Outlook().MasterCategoriesById(&outlookCategoryId).Get(options)


```