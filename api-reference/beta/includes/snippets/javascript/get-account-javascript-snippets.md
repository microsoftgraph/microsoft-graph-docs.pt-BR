---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb9b9af85baa3bf0246d4b5c4052a3b980ef2a19e5f8194980c652f014bfe794
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let account = await client.api('/me/profile/account')
    .version('beta')
    .get();

```