---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8af265145f26d98cf069bd965451cfd672625cdb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951526"
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