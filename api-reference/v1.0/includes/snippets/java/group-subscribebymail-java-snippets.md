---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c29a7c714fb028a915567cc2c18089b45d24ed5f5cc0b05fde69f544cf22f3f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329710"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .subscribeByMail()
    .buildRequest()
    .post();

```