---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c859c702b7573648843ab8a2d85ddf9987d42d5e61d8bb7bede13bafee18b1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.Notebooks["{notebook-id}"].SectionGroups
    .Request()
    .GetAsync();

```