---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a57c3bb46f1f78b05f70e2dce98bf32ecaf3c959957ec662b623b2be3d069f55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272365"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = await graphClient.Me.ContactFolders["{contactFolder-id}"]
    .Request()
    .GetAsync();

```