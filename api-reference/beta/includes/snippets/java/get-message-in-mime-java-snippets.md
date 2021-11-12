---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32ea2a3f673782ac8b7e3a1ab4fd59374046d6f88a3de9c0cc1ff485f2f0ba73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328041"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.me().messages("4aade2547798441eab5188a7a2436bc1").content()
    .buildRequest()
    .get();

```