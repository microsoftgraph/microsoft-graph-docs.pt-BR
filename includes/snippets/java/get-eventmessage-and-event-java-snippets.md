---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 194818abc0d2611daa9b32a5d5f7045053c9628a97154f69e2cf63557c81ec07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129726"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADADVj3fyAABZ5hYdAAA=")
    .buildRequest()
    .expand("eventMessage/event")
    .get();

```