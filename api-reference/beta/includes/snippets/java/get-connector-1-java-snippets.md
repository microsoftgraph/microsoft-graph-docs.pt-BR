---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a08de17a81fb7fac4e79f6eac7eef1c79c409f17
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211005"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Connector connector = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors("{id}")
    .buildRequest()
    .get();

```