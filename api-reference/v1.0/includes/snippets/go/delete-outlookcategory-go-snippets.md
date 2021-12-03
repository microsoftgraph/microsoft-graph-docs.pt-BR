---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62968500c1e4aa550c5c00e0252c45a54fd48a87
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286019"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

outlookCategoryId := "outlookCategory-id"
graphClient.Me().Outlook().MasterCategoriesById(&outlookCategoryId).Delete(nil)


```