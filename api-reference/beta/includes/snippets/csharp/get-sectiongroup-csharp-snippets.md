---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19a39973033cd22b8c5833a190470c360892e382c7b3fe314b68a4cc1d5b3318
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216684"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = await graphClient.Me.Onenote.SectionGroups["{sectionGroup-id}"]
    .Request()
    .GetAsync();

```