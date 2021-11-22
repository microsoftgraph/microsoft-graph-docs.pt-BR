---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 566ae43c4dc5c8bde54763e37079c1a9e89331736143c7edd03afee7a976357b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273227"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.termStore().sets("{setId}")
    .buildRequest()
    .delete();

```