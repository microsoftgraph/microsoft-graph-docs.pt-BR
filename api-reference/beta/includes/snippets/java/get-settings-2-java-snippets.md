---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 360a3d8fe9f47fd48879b942ea7037420c3b93c3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209969"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Settings settings = graphClient.customRequest("/me/analytics/settings", Settings.class)
    .buildRequest()
    .get();

```