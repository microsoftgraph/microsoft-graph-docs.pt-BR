---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5cf694db5c1ec8353b818aafb8ec94ad9ec3079966ced4495480acfa8d9b4254
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329694"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .get();

```