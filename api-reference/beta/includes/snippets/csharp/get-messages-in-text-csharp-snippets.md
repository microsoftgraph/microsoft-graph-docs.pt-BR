---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7daf0a4f0042443b4e4c1cab9bca247911d72a279d3fe2dca83bd6d940e654e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select("subject,body,bodyPreview,uniqueBody")
    .GetAsync();

```