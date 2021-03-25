---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9c0c0953ba173677acafd82e710274a386986ec
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208442"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApprovalCollectionPage privilegedApproval = graphClient.privilegedApproval()
    .buildRequest()
    .get();

```