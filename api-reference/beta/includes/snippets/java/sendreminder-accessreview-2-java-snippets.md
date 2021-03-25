---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7749a0916c6ee4b8a86eff9bba9258fd7167130
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209465"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("04e5c3b2-9db2-40d3-a204-128f4956ae8e").instances("70463350-742e-4909-bfa5-bc23447bd002")
    .sendReminder()
    .buildRequest()
    .post();

```