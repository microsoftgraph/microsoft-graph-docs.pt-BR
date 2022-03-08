---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 748c5907b6d485c4be97e21c606741d565b4b2cf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334622"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyServicePrincipalHistoryItemCollectionPage history = graphClient.identityProtection().riskyServicePrincipals("{riskyServicePrincipalId}").history()
    .buildRequest()
    .get();

```