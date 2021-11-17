---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0bd73fe1e299d7b22d3f82da3a19fad89d72b2a2a5965f928bfc9784ecd0320
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedMembers = await graphClient.DirectoryRoles["{directoryRole-id}"].ScopedMembers
    .Request()
    .GetAsync();

```