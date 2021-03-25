---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b8946787bd7c3c443495e1a075b62018391ac11
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208184"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contract contract = graphClient.contracts("{id}")
    .buildRequest()
    .get();

```