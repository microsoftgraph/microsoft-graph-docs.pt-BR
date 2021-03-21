---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32cfd2d12ec0265bd1f8c8d3013bde59e609edff
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966516"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directoryObjects("{id}")
    .buildRequest()
    .get();

```