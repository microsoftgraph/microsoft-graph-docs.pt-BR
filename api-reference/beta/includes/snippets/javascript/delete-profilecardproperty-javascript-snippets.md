---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5af4039efd4fcca8ee9c8725b1a3fa2451119d9c
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080675"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/settings/profileCardProperties/fax')
    .version('beta')
    .delete();

```