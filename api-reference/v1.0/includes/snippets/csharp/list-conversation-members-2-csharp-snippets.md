---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 080cfe2d99655b51a73b96a70c6b77854976ad0c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Chats["{chat-id}"].Members
    .Request()
    .GetAsync();

```