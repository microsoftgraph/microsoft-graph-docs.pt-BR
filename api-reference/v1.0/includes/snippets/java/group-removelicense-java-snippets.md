---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c69212d0a0b918e13666bb830312b158eaecc92a
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953660"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> addLicensesList = new LinkedList<String>();

LinkedList<String> removeLicensesList = new LinkedList<String>();
removeLicensesList.add("skuId-value-1");
removeLicensesList.add("skuId-value-2");

graphClient.groups("1ad75eeb-7e5a-4367-a493-9214d90d54d0")
    .assignLicense(addLicensesList,removeLicensesList)
    .buildRequest()
    .post();

```