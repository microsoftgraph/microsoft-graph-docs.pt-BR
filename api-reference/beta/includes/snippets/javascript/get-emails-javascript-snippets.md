---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d61dbc550014ad2b77277480641b575e84de27de
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996948"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/emails')
    .version('beta')
    .get();

```