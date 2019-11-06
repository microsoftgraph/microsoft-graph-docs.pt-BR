---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb016ebb824bb3047af158c14cb33ad678f90b33
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/positions/{id}')
    .version('beta')
    .delete();

```