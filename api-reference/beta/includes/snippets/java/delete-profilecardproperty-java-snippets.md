---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f375e3cecd085fe49d7f33749f5db73a63782e337168f4b6346827d50c155895
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099521"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.organization("{organizationId}").settings().profileCardProperties("fax")
    .buildRequest()
    .delete();

```