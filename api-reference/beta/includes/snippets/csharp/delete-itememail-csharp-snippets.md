---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c66fa9346344765801cd20b0c54cedeaf14b53cc779b419aba563858fc2bb03e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Emails["{itemEmail-id}"]
    .Request()
    .DeleteAsync();

```