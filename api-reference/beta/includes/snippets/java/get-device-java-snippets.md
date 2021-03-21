---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b87e3fccfc44742cde8c17a966dc29b1b79b6852
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980305"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = graphClient.devices("{id}")
    .buildRequest()
    .get();

```