---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 977d15e0435dc59a0789604e64f0891e1020b8a1e1997ae95a84a42c568c698a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/messages')
    .version('beta')
    .select('sender,subject')
    .get();

```