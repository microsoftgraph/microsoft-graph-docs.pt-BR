---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1eebc53c3a10bde26755c075286e63983c7b385
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999105"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/owners')
    .get();

```