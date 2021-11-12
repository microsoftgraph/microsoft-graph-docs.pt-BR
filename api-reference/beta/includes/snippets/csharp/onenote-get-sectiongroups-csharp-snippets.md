---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95c8dc18e7500d5586b4ec9886f210f723ae60da98fd14dc48fea27ca587ff2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.SectionGroups
    .Request()
    .GetAsync();

```