---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31bc08bd93f998e77c57159dc4b4989c32ad17b3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
identityUserFlowAttributeAssignmentId := "identityUserFlowAttributeAssignment-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserAttributeAssignmentsById(&identityUserFlowAttributeAssignmentId).Delete(options)


```