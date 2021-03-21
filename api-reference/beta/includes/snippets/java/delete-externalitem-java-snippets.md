---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb310d847c93683dde290ee303282a7c53b58d70
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983837"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.connections("contosohr").items("TSP228082938")
    .buildRequest()
    .delete();

```