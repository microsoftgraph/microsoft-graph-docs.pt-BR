---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc521606855b0f22102e729670a557a02541c9706e4dbc30ec7423eb3159e806
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["{mailFolder-id}"].MessageRules["{messageRule-id}"]
    .Request()
    .DeleteAsync();

```