---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 001d04e0f55542cc909eb2fd12fb4b31480a705bb64368ba9cbb99b044c10aab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let passwordMethods = await client.api('/me/authentication/passwordMethods')
    .version('beta')
    .get();

```