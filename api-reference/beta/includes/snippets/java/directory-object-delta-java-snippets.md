---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 553b94f0b1ec26bb47645ca388a97d941904f752
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946618"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directoryObjects("delta")
    .buildRequest()
    .get();

```