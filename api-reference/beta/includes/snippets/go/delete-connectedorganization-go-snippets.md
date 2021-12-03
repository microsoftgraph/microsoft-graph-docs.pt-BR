---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73297efa546628926b0e12bde50eea1feeefdbca
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286135"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

connectedOrganizationId := "connectedOrganization-id"
graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).Delete(nil)


```