---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ffb4af9779ba248511d5d5828abd97e4acf0c3d
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580063"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.connections("contosohr")
    .buildRequest()
    .delete();

```