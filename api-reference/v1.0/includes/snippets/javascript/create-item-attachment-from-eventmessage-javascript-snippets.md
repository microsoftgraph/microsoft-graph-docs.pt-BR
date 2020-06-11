---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed85cfc98825062fc0592e885fccd44b76f605dd
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.ItemAttachment",
  name: "name-value",
  item: "{message or event entity}"
};

let res = await client.api('/me/events/{id}/attachments')
    .post(attachment);

```