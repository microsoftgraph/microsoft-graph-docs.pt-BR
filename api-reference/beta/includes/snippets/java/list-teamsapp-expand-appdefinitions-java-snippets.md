---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 368ec09fd0720b95a317eb5865ae255593c16efb
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689290"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("id eq '876df28f-2e78-423b-94a5-44181bd0e225',")
    .expand("appDefinitions")
    .get();

```