---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 756d60545bc6cf9576d0c60167feb8460bdd0c0d5017f05acb9a921ef558dd6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/me/classes')
    .version('beta')
    .get();

```