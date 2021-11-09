---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e82844ef0d07d6fc2dbbba5d18b0fa7e21c15671
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getApplicableContentTypesForList = await client.api('/sites/{siteId}/getApplicableContentTypesForList(listId='{list-id}')')
    .version('beta')
    .get();

```