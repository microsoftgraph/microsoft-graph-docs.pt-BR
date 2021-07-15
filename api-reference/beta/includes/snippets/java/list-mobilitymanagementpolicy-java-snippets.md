---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffa4c2ddcd412e2ecba5aaeaf45a4b6a155ecbe3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440861"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MobilityManagementPolicyCollectionPage mobileAppManagementPolicies = graphClient.policies().mobileAppManagementPolicies()
    .buildRequest()
    .get();

```