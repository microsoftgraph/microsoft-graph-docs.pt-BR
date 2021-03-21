---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f56d8c6b3a0c493c812d8c0a6a87521d8a2f9c6b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954630"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InformationProtectionLabelCollectionPage labels = graphClient.me().informationProtection().policy().labels()
    .buildRequest()
    .get();

```