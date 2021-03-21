---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6966bea1c7d085dfa77c4db6f0de3f265b4ac915
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976755"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProjectParticipationCollectionPage projects = graphClient.me().profile().projects()
    .buildRequest()
    .get();

```