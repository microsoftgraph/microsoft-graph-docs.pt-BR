---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79059a01fe46f087d1552465e2b47174b2444b8927be94a2e23ffe465a934088
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899803"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplate = await graphClient.DirectorySettingTemplates["{directorySettingTemplate-id}"]
    .Request()
    .GetAsync();

```