---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23889ffde13b0dfe46f3b1c43e3bff3ad05ebbdd5eee77f9c5f5252ef6ed0b63
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159874"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teamwork().workforceIntegrations("{workforceIntegrationId}")
    .buildRequest()
    .delete();

```