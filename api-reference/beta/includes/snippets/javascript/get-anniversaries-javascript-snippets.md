---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 189e3cd64ebb925cbac8b43af9c272f604ec39eb
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/anniversaries')
    .version('beta')
    .get();

```