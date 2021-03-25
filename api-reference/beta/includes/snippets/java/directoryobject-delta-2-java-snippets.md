---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfc7cb2a9c1a88497fc497acca5cd21861a52cc2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209261"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directoryObjects("delta")
    .buildRequest()
    .filter("isOf('Microsoft.Graph.User') or isOf('Microsoft.Graph.Group')")
    .get();

```