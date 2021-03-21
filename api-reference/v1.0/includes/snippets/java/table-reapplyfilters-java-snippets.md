---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f319d6e3d301c4e5d5f5c35bdeea8364d42580d9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973161"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .reapplyFilters()
    .buildRequest()
    .post();

```