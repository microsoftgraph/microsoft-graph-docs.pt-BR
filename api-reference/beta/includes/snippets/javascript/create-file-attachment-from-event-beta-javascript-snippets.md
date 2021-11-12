---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0e65a9fec0e8ec7ac02413874d121237d08b6fdb8634b7f6217439f7ca88826
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    '@odata.type': '#microsoft.graph.fileAttachment',
    name: 'menu.txt',
    contentBytes: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk='
};

await client.api('/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments')
    .version('beta')
    .post(attachment);

```