---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfef309adb36015bcc9d0df7519041215251f49f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090775"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).TokenIssuancePolicies().Get(options)


```