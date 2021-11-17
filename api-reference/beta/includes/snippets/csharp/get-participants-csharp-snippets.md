---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9029096783d56c5325bdd3d7f6caa38ab7dcc610059794d77f05041bcc77a6c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = await graphClient.Communications.Calls["{call-id}"].Participants
    .Request()
    .GetAsync();

```