---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40a23176dd4322b9a9aaf6b51a674736d947bf06
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220215"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .filter("startsWith(appDisplayName,'Azure')")
    .top(10)
    .get();

```