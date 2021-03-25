---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52a4975c0e8673dd52c2214b10e518481499b7e5
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208247"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobCollectionPage jobs = graphClient.print().printers("{id}").jobs()
    .buildRequest()
    .get();

```