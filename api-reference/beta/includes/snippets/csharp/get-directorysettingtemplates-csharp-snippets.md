---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98e625b910e4df40952a545b05b9b5e4ce24bb61
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608878"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplates = await graphClient.DirectorySettingTemplates
    .Request()
    .GetAsync();

```