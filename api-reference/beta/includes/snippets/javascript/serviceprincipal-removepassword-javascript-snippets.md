---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56b1a882dba5413ae4871d4ae38ae617efd6c1bb
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removePassword = {
    keyId: "f0b0b335-1d71-4883-8f98-567911bfdca6"
};

let res = await client.api('/servicePrincipals/{id}/removePassword')
    .version('beta')
    .post(removePassword);

```