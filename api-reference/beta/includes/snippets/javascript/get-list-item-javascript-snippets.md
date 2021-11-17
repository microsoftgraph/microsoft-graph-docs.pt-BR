---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6e599826c57f638c438bc73712827d27ea03e4cc1af2e2e886d20c45fa4317d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let listItem = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields')
    .version('beta')
    .get();

```