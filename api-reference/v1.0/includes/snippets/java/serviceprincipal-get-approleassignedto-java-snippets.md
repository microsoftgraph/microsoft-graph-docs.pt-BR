---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2c51d9580dcbdadde063df9905351654fda0c4d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981878"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignedTo = graphClient.servicePrincipals("8e881353-1735-45af-af21-ee1344582a4d").appRoleAssignedTo()
    .buildRequest()
    .get();

```