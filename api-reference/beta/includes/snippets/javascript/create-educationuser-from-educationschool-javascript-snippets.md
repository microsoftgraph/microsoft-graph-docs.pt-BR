---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 318c0d823523ae2511c6de20231478ad997c9d52
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712573"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/beta/education/users/14008"
};

let res = await client.api('/education/schools/{id}/users/$ref')
    .version('beta')
    .post({educationUser : educationUser});

```