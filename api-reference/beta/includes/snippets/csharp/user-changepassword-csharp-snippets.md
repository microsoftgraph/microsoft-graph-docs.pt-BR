---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac2b1ad276c7df132bd80ed62b78c56621b517e7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var currentPassword = "xWwvJ]6NMw+bWH-d";

var newPassword = "0eM85N54wFxWwvJ]";

await graphClient.Me
    .ChangePassword(currentPassword,newPassword)
    .Request()
    .PostAsync();

```