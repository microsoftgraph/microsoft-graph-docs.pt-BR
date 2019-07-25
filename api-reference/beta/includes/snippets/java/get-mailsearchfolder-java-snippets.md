---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab67980607e8e777aa080dabb760582c5c2e1643
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880088"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = graphClient.me().mailFolders("AAMkAGVmMDEzN")
    .buildRequest()
    .get();

```