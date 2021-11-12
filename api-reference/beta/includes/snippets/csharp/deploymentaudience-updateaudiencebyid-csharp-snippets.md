---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4a3253e35272b4c028b38fb88810b975ed1c91bbd3f2df29da4368bf512e908
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159568"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberEntityType = "String";

var addMembers = new List<String>()
{
    "String"
};

var removeMembers = new List<String>()
{
    "String"
};

var addExclusions = new List<String>()
{
    "String"
};

var removeExclusions = new List<String>()
{
    "String"
};

await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"].Audience
    .UpdateAudienceById(memberEntityType,addMembers,removeMembers,addExclusions,removeExclusions)
    .Request()
    .PostAsync();

```