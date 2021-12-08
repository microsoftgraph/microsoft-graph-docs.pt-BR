---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 169d6d0a38a1179e2bf939dca613e14e1f845070
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346014"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().PeopleInsights().Get(nil)


```