---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c90fc3e4a6e706a8acdabea66eddd65dffb277221b33dc71f0098bc6c9b718bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: 'Display name'
};

await client.api('/applications')
    .post(application);

```