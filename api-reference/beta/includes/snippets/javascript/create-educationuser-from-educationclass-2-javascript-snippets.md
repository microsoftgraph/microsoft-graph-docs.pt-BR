---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b09a460afd91fee7a98ff193c4480f84a498de1bc8fde798fc6f09e8cf23cc1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215174"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/beta/education/users/14011'
};

await client.api('/education/classes/11017/teachers/$ref')
    .version('beta')
    .post(educationUser);

```