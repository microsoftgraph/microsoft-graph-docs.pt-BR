---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a36ac4b674a6118a4c82c050f4541516e6547e26da1ec23c92b01e7bcb137011
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272284"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SkillProficiencyCollectionPage skills = graphClient.me().profile().skills()
    .buildRequest()
    .get();

```