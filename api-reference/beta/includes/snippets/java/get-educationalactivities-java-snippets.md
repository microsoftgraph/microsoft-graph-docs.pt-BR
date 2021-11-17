---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9442d3d1f4c036a9a7edff43be43f281da0f7cb600301885a1ad6c720778fb6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214614"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationalActivityCollectionPage educationalActivities = graphClient.me().profile().educationalActivities()
    .buildRequest()
    .get();

```