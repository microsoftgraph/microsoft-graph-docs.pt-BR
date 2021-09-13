---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d384cc377ec6463aaf03edf6612b632387355ac1e85d386ee16634d64e17d63c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conditionalAccessPolicy = await client.api('/identity/conditionalAccess/policies/{id}')
    .get();

```