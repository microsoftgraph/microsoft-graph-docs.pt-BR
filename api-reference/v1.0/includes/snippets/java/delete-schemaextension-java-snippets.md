---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61e5fe1bcb063adf0d7467915b709c63c0aa5a510980e2be67e2331423cfb4c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215248"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.schemaExtensions("{id}")
    .buildRequest()
    .delete();

```