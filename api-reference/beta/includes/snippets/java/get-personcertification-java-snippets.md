---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36b45be91e991a5f9422a72dd7ffce35c1356db452deaf0873b85035ebcc2aa9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215560"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCertification personCertification = graphClient.me().profile().certifications("{id}")
    .buildRequest()
    .get();

```