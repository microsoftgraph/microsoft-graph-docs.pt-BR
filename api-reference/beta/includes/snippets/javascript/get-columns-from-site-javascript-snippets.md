---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f5ec0fbf2879a42402c74c6c0a363431d6219a9cb4788b8e89b082dadaafea7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159757"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/columns')
    .version('beta')
    .get();

```