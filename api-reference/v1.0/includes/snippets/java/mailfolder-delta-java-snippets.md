---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99fce0b870f2767230b095a3932a73c360adcbc0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893128"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderDeltaCollectionPage delta = graphClient.me().mailFolders()
    .delta()
    .buildRequest()
    .get();

```