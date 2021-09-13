---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a99cd27f133a7e5cae0010691aa8d155c0b957092050f3f976187c618b22a9c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': '#microsoft.graph.fileAttachment',
  name: 'smile',
  contentBytes: 'R0lGODdhEAYEAA7'
};

await client.api('/me/messages/AAMkpsDRVK/attachments')
    .post(attachment);

```