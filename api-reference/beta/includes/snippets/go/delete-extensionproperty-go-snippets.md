---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3a64d4809a9cd9794ba0ccb45f46305d9ae7496
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285820"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
extensionPropertyId := "extensionProperty-id"
graphClient.ApplicationsById(&applicationId).ExtensionPropertiesById(&extensionPropertyId).Delete(nil)


```