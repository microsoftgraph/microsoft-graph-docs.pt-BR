---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 323cec7db071c209425dd2bee7f77228c9bb71b01805bb5e513cf0ca512b5fa8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/beta/education/users/14008'
};

await client.api('/education/schools/{id}/users/$ref')
    .version('beta')
    .post(educationUser);

```