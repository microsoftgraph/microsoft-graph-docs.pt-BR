---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a1ac1fb1c0f2d86559949fbca379f2cdd99ad8a1fc85a4461c276ad0bc914c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216290"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .get();

```