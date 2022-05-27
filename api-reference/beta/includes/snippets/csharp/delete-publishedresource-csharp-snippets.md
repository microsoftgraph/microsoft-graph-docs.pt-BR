---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f351644760426415231f5c91a37ae531155ef016f7e0ab37c81eb55faa4e2fae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].PublishedResources["{publishedResource-id}"].AgentGroups["{onPremisesAgentGroup-id}"].Reference
    .Request()
    .DeleteAsync();

```