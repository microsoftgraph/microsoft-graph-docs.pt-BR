---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c07b512218f322586465526b4063978d7db271553b89d6040dffc713df2d1141
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274694"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage monthlyPrintUsageByUser = graphClient.print().reports().monthlyPrintUsageByUser()
    .buildRequest()
    .get();

```