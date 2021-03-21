---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8672d6457f53583db20b193d007f90dd893c2ce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977574"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformation userAccountInformation = graphClient.me().profile().account("{id}")
    .buildRequest()
    .get();

```