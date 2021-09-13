---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43551cbaf9c4f7466d7e33395262ecc178c99b9f53ddc0d7f91def1e70f75b18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215305"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationTemplate applicationTemplate = graphClient.applicationTemplates("{id}")
    .buildRequest()
    .get();

```