---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61ea7640a6f4a46c4a54be9894bce1db0abf5c8d
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507705"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Notebook notebook = new Notebook();
notebook.displayName = "My Private notebook";

graphClient.me().onenote().notebooks()
    .buildRequest()
    .post(notebook);

```