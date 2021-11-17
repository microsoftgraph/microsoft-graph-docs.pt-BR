---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25bb1fa8db6a1dfc840b88e669f420a1499d90c96b4d409fd828b5b1c9edbac1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273205"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.termStore().sets("{setId}").terms("{termId}")
    .buildRequest()
    .delete();

```