---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59ec6259bf8c5256badb8d184a45893c907535eb24c20e2a01e1e3cecce7db44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273281"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/awards/{personAwardId}')
    .version('beta')
    .delete();

```