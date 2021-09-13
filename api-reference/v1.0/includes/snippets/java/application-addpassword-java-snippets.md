---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3342d8551b0e68381c4065532efd1535e6218711d3f3ee9cfe2d1f696634ba95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329204"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.displayName = "Password friendly name";

graphClient.applications("{id}")
    .addPassword(ApplicationAddPasswordParameterSet
        .newBuilder()
        .withPasswordCredential(passwordCredential)
        .build())
    .buildRequest()
    .post();

```