---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb5fa6d26c7432a313f108d3090679af67ceba15dee43b15c41d00637e3672db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/education/me/user')
    .version('beta')
    .get();

```