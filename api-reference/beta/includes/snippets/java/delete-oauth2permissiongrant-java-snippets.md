---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac9c53f042ebcda17faa756cce6517046b0ea31b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758704"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.oauth2PermissionGrants("l5eW7x0ga0-WDOntXzHateQDNpSH5-lPk9HjD3Sarjk")
    .buildRequest()
    .delete();

```