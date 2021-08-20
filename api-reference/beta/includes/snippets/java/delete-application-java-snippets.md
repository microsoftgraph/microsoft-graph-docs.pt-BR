---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 575aab17be18c85393f519a7d50111dc52ded482efe46893aad39f2b9cd0abb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156524"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}")
    .buildRequest()
    .delete();

```