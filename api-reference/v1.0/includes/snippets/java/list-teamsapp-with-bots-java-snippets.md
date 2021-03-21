---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92499424896fb6f70030c54248b38f810b383a43
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976767"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("appDefinitions/any(a:a/bot ne null)")
    .expand("appDefinitions($expand=bot)")
    .get();

```