---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1c5d93246a48db0758bd34a7472bb05bed91471261d886196610370927ffe0e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326941"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String key = "Base64-encoded-pfx-content";

String password = "password-value";

graphClient.trustFramework().keySets("{id}")
    .uploadPkcs12(TrustFrameworkKeySetUploadPkcs12ParameterSet
        .newBuilder()
        .withKey(key)
        .withPassword(password)
        .build())
    .buildRequest()
    .post();

```