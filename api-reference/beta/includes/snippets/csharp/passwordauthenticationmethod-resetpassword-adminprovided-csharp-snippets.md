---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee4ca959dab480b7a23f0286fd6e161a14d2bc9f
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805987"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newPassword = "newPassword-value";

await graphClient.Users["{id}"].Authentication.PasswordMethods["{id}"]
    .ResetPassword(newPassword,null)
    .Request()
    .PostAsync();

```