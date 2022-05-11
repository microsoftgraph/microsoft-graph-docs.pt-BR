---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8d8be883473347ec3c11894104366d44450066b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325002"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userAccountInformationId := "userAccountInformation-id"
graphClient.Me().Profile().AccountById(&userAccountInformationId).Delete()


```