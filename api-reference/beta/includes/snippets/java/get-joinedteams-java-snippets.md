---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c79d182f7f9b42633a5352fbca0e61c6ed682f5
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49530530"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamCollectionWithReferencesPage joinedTeams = graphClient.me().joinedTeams()
    .buildRequest()
    .get();

```