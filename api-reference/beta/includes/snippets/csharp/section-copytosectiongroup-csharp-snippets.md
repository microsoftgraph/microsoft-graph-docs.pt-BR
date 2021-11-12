---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc2b6ea0d8b02e219807583d3dd1633e5968ce079f4980f78605853def595883
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "id-value";

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Sections["{onenoteSection-id}"]
    .CopyToSectionGroup(id,groupId,renameAs,null,null)
    .Request()
    .PostAsync();

```