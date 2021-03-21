---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66b680113d5bb843d3d9eb809c289b1f9f0eba50
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966561"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsite personWebsite = graphClient.me().profile().websites("{id}")
    .buildRequest()
    .get();

```