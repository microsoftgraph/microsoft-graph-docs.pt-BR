---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62a8e664c53bcca8b3870c79c126e0b6ff3e1ebc9fd34966d04c07b14b1741e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["{message-id}"]
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select("subject,body,bodyPreview,uniqueBody")
    .GetAsync();

```