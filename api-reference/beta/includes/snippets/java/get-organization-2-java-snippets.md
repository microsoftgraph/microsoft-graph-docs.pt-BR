---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62612c5e38fd5ca4569060bbc3124725d24a58de1ca8534d17257a812b3aabde
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160077"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationCollectionPage organization = graphClient.organization()
    .buildRequest()
    .get();

```