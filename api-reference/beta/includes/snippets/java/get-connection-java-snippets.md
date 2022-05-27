---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eacc10081f4e39fcc66a91e8aa24ca2dcb0da96d
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719144"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectionQuota connectionQuota = graphClient.external().connections("contosohr").quota()
    .buildRequest()
    .get();

```