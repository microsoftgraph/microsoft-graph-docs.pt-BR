---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57e4ebb1fb0a9a504cef4a0f3647c03c793071a69b514e4dd39d6dfea638e006
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213745"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobCollectionPage jobs = graphClient.print().shares("{id}").jobs()
    .buildRequest()
    .get();

```