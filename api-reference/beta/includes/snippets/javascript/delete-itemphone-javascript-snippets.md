---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02dafb7d7a7dfe4aafcfa60092090482bba341cf
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/phones/{id}')
    .version('beta')
    .delete();

```