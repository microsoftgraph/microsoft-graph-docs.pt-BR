---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10b0b182f2c9a9082625e8e3750f0f98c2969531633b13e531bd1b6752265f59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898897"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["{message-id}"].Attachments["{attachment-id}"]
    .Request()
    .GetAsync();

```