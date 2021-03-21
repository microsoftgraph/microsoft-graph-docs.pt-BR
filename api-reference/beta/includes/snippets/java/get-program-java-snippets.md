---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52396ac24a7b6fcb19f981862dd1ef2917fd7b99
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968145"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramCollectionPage programs = graphClient.programs()
    .buildRequest()
    .get();

```