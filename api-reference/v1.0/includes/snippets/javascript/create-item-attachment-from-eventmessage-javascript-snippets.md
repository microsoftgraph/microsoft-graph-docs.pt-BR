---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1dca71830038015068dd5805e4e0e0552cb7c620
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.ItemAttachment",
  name: "name-value",
  item: {
    @odata.type: "microsoft.graph.message"
  }
};

let res = await client.api('/me/events/{id}/attachments')
    .post(attachment);

```