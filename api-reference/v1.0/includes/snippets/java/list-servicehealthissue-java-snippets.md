---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74f769a54cc5275bf2dff83959956d0321d1e70d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58260797"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthIssueCollectionPage issues = graphClient.admin().serviceAnnouncement().issues()
    .buildRequest()
    .get();

```