---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7015d3384b21afd42072e47f3959bfb447ed56c0d9aca34404aa74bc5f3afd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07')
    .version('beta')
    .delete();

```