---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49264ce2eca6d188f6ea0d293bc8ef072f6c04626289092e0febd5e8971677df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/me/messages/{id}/attachments')
    .get();

```