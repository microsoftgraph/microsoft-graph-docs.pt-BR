---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97e2bf98131c1fcafe5d299df1ceac332cbe511ffa0547146075b6bc19c7791e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101737"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10001").classes("11001")
    .buildRequest()
    .delete();

```