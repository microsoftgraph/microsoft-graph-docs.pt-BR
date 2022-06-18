---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73352b85fc9b65c7cea4c720579191b270e56024ab6b30487a8aac0836309556
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216944"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}").jobs("{id}")
    .cancel()
    .buildRequest()
    .post();

```