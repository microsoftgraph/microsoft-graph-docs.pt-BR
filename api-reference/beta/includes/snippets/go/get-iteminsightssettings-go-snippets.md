---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22016d0ab9e1b20fc55b15324409f7b4803276d5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020814"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ItemInsights().Get(options)


```