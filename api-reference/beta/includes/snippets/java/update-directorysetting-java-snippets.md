---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5fe83738a6863c5084eccd92b0fb6ccdeb1095cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973482"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = new DirectorySetting();
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "name-value";
values.value = "value-value";
valuesList.add(values);
directorySetting.values = valuesList;

graphClient.settings("{id}")
    .buildRequest()
    .patch(directorySetting);

```