---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03b6d68fe88fcf22e051e156a0af8d3addb53bbd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979033"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.settings("{id}")
    .buildRequest()
    .delete();

```