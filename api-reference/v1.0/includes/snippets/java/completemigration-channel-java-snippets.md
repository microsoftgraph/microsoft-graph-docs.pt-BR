---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c65425b547c012493630bb844bf47210e8983d415e32e20bfef56a037adcb6f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329293"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels("19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2")
    .completeMigration()
    .buildRequest()
    .post();

```