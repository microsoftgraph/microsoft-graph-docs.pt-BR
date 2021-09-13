---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0511495d211c78bb2d50c985153d546eab079dde115c7db7e5518bf3883ecc59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
  color: 'preset15'
};

await client.api('/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac')
    .update(outlookCategory);

```