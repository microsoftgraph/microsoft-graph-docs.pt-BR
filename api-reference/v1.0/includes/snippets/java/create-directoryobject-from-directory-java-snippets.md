---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba4e85468dcb29bdbde58aacede28fd5bcb1c85cfb5a8a3e4b08b2507eb817e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103060"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("{object-id}")
    .restore()
    .buildRequest()
    .post();

```