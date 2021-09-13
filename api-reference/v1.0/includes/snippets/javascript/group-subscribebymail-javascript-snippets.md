---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d689bbfd71453367a0251c3ff8e201304f4c58f8cbac6aefe18c79f3dfbea767
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/subscribeByMail')
    .post();

```