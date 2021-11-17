---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10964d0f4e7bb2c2a091552b7b38dce0402380598eb3d4ab8c15786d82918707
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102274"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonInterest personInterest = graphClient.me().profile().interests("{id}")
    .buildRequest()
    .get();

```