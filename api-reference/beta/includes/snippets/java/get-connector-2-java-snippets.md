---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07155a3582083db1ebe83a210ae8a5715a02fa9e8c7f952cfe4146c5f7c5d32e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157716"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnector printConnector = graphClient.print().connectors("{id}")
    .buildRequest()
    .get();

```