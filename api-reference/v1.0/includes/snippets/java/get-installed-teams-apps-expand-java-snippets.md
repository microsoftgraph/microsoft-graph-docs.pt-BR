---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 434a0a4a4f2dc71c55ebd1241161db0f18303d15
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893198"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsAppInstallationCollectionPage installedApps = graphClient.teams("{id}").installedApps()
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```