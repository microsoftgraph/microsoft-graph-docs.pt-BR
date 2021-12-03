---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39b955dec8295be76c2640c6ddd3153d31ee10f8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287004"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
profileCardPropertyId := "profileCardProperty-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ProfileCardPropertiesById(&profileCardPropertyId).Get(nil)


```