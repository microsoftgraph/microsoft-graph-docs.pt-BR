---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37d76f9f6bf2c9497b971923701bcba042c256d08d7c453592acf10fe08a519c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216360"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/{id}'
};

await client.api('/groups/{group-id}/members/$ref')
    .version('beta')
    .post(directoryObject);

```