---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b75faf5fe7e5e5c954315c61bbc3f8f18cf4f673a1c88451f52a2445ba8a28e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157051"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserCollectionPage riskyUsers = graphClient.identityProtection().riskyUsers()
    .buildRequest()
    .filter("riskLevel eq microsoft.graph.riskLevel'medium'")
    .get();

```