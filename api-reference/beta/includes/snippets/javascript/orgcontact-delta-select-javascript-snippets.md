---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efdd5f98aa119282f876be13219f3aad1b8d51f8d180b31540dd5e9f2b357df5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .version('beta')
    .select('displayName,jobTitle,mail')
    .get();

```