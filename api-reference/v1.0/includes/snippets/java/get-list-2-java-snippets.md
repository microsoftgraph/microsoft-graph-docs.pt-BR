---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1178723a2a1976a9cb6f086a511421788cc47aeb8a75c4037df854c1e2c30de7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157318"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{site-id}").lists("{list-title}")
    .buildRequest()
    .get();

```