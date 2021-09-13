---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 887893cb52d08fe7291b0c7e1b5a5d8ed61679f608e35ea954be4448a932cd37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271999"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Users["{user-id}"].Presence
    .Request()
    .GetAsync();

```