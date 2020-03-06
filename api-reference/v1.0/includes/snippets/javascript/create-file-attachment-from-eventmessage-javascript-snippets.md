---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19b83c0a85fb4dd8b60d4801b7209a5db2885219
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "microsoft.graph.fileAttachment",
  name: "name-value",
  contentType: "contentType-value",
  isInline: false,
  contentLocation: "contentLocation-value",
  contentBytes: "base64-contentBytes-value"
};

let res = await client.api('/me/messages/{id}/attachments')
    .post(attachment);

```