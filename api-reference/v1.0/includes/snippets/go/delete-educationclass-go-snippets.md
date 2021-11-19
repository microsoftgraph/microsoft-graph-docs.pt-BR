---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7cddffa0d157f36e090ef83b439e43b99818f330
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098974"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).Delete(options)


```