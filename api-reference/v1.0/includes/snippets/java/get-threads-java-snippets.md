---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc82da028ac9d036ef14453c1e6d4cd7081d75c8d74f9ff445601fbda88fc24e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103063"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThreadCollectionPage threads = graphClient.groups("{id}").conversations("{id}").threads()
    .buildRequest()
    .get();

```