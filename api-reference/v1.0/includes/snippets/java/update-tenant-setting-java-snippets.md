---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de5dee8e83c3e9c529bd1a810beb5d72c191ee8c
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514625"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = new GroupSetting();
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "AllowToAddGuests";
values.value = "false";
valuesList.add(values);
groupSetting.values = valuesList;

graphClient.groupSettings("f0b2d6f5-097d-4177-91af-a24e530b53cc")
    .buildRequest()
    .patch(groupSetting);

```