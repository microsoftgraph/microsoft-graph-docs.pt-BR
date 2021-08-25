---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97a4a977ccf309bf5c1e5b2478ea6cd4b68f62d8cda59bf2aa6c1d52846ba49d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217094"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/conversations/{id}')
    .delete();

```