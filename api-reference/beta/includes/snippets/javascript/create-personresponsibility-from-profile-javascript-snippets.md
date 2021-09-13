---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91e0ad2e8d1bde66f9b87c1a5fef1e21b8379b678cd564345d10915f3fbcb48b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  description: 'Member of the Microsoft API Council',
  displayName: 'API Council',
  collaborationTags: [
    'askMeAbout'
  ]
};

await client.api('/me/responsibilities')
    .version('beta')
    .post(string);

```