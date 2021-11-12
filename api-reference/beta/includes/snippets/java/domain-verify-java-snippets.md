---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21cfeb4d3435ef5434560ac84d7862f5400a1be206f2ed6e9618204955e7a94a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214203"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("contoso.com")
    .verify()
    .buildRequest()
    .post();

```