---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2e83054aebaeb6d179c5b411eab53e241c42c15
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997292"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = await graphClient.Me.Profile.Languages["{id}"]
    .Request()
    .GetAsync();

```