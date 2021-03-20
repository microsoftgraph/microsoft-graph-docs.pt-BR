---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 870174d9d2a61d2c0841ddec75cc03fa189f4f8f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978834"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .delete();

```