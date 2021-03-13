---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8eee1f956f9265fadd4f9366240bce2783e30cd9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    '@odata.type': '#microsoft.graph.referenceAttachment', 
    name: 'Personal pictures', 
    sourceUrl: 'https://contoso.com/personal/mario_contoso_net/Documents/Pics', 
    providerType: 'oneDriveConsumer', 
    permission: 'Edit', 
    isFolder: 'True' 
};

await client.api('/me/messages/AAMkAGE1M88AADUv0uFAAA=/attachments')
    .version('beta')
    .post(attachment);

```