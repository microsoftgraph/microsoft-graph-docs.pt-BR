---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce36d18e3f75e9a10888db1e0a305bd049f552665c45eb262ba18eae03d5614a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100251"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = graphClient.education().users("{user-id}")
    .buildRequest()
    .get();

```