---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f4144237cafe1780aac6350dc5c87868c66518d379cb8e4c550f6c1a650a846
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157993"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personInterest = await client.api('/me/profile/interests/{id}')
    .version('beta')
    .get();

```