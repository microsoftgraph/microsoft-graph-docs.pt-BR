---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0eda06646ab6e13fae87ba85cbc3ade043214f4a12879cab38786a2ab550dd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .GetAsync();

```