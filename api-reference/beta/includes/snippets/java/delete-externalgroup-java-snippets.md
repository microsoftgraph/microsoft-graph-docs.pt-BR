---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5ba417b7ec2b0c69e972b62a43eb1e530131bcb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981023"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.external().connections("contosohr").groups("31bea3d537902000")
    .buildRequest()
    .delete();

```