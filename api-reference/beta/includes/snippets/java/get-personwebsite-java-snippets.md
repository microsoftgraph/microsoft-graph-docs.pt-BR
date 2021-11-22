---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 404ca33f52b967cbb61cd19ae64759adc1708cf5ac16608c5021094d2f065f92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327413"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsite personWebsite = graphClient.me().profile().websites("{id}")
    .buildRequest()
    .get();

```