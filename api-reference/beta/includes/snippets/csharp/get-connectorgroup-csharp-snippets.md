---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 011a7e83233e4d16aa52f7e238d8021d5357c41baf6f056bbe213b5b8a51fedd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups["{connectorGroup-id}"]
    .Request()
    .GetAsync();

```