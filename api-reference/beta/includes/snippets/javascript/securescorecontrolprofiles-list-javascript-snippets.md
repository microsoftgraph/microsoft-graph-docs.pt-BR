---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbd3e176e5f75a1b88267f3b3f406c4f25bb921ca92e3cb3a36e39119ec07968
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329325"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScoreControlProfiles = await client.api('/security/secureScoreControlProfiles')
    .version('beta')
    .get();

```