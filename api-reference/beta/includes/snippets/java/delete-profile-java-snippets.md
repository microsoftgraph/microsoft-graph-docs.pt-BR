---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 402750f3f2eaf8960641c01d9a8fb34668857e880aa3f8599a4463505b4936ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326651"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile()
    .buildRequest()
    .delete();

```