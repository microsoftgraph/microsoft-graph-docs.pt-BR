---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34d4fa4a4c6f600e79a41e08d2dbb508c1ae21481b4eea37adcd80a3ea162c9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899799"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplates = await graphClient.DirectorySettingTemplates
    .Request()
    .GetAsync();

```