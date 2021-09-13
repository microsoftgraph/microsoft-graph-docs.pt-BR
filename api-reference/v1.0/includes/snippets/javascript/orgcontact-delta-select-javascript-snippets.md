---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb7905980e7edd0309ca5647a9eb05994945f23858358b3db9d6adc2115b216b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .select('displayName,jobTitle,mail')
    .get();

```