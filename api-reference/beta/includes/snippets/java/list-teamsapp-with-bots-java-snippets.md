---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e65f0529d4397e502d499bf9ca0e3024a78d73b8
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844134"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("appDefinitions/any(a:a/bot ne null)")
    .expand("appDefinitions($expand=bot)")
    .get();

```