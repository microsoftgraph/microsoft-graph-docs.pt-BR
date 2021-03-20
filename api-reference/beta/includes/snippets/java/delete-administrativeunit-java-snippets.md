---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5b7146037a9a0e3eb2e4129ca93bf6c79ba4758
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966985"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.administrativeUnits("{id}")
    .buildRequest()
    .delete();

```