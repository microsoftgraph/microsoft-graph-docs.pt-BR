---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1ac4c28a87ad4221890fc8f5974d39919ac4148
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983886"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShareCollectionPage shares = graphClient.print().shares()
    .buildRequest()
    .get();

```