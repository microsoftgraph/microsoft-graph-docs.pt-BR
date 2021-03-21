---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8aed909d0d46a2f7d9c93393e1223d7993a52ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983378"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.teams("{id}").channels("{id}").filesFolder()
    .buildRequest()
    .get();

```