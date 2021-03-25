---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1ac4c28a87ad4221890fc8f5974d39919ac4148
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210440"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShareCollectionPage shares = graphClient.print().shares()
    .buildRequest()
    .get();

```