---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8fadf509818616d8aa452df7d85a58bd4b19bb99
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': 'microsoft.graph.fileAttachment',
  name: 'name-value',
  contentType: 'contentType-value',
  isInline: false,
  contentLocation: 'contentLocation-value',
  contentBytes: 'base64-contentBytes-value'
};

await client.api('/me/messages/{id}/attachments')
    .post(attachment);

```