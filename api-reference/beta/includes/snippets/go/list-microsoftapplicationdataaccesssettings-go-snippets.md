---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce0fe6a923c442e222096cc0264157f37bcaa6df
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324123"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().MicrosoftApplicationDataAccess().Get()


```