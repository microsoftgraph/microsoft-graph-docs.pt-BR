---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc7f644f0a518ab26b71b812613be2d46e3dde81699ad6bb00cf7274819dae50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157014"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationalActivity educationalActivity = graphClient.me().profile().educationalActivities("{id}")
    .buildRequest()
    .get();

```