---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af21757a1dcab99b9f58caa11e79c0accb877ef8
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690331"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'")
    .get();

```