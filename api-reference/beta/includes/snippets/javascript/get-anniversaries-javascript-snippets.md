---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 153505cfa5302a7c24c5f15aee3a2d45a5a04c1a968502af2864cccb24083621
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let anniversaries = await client.api('/me/profile/anniversaries')
    .version('beta')
    .get();

```