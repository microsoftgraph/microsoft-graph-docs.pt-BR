---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b8a3e53dc421d85bf3499d3f3b4370d4a2a87fcbea0b19ce300f761d7d264a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let place = await client.api('/places/bldg1@contoso.com')
    .get();

```