---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ae44c69f984831735e9aea27a445ce9d80d7da7ca0d8f32242b62d2b8874e8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shares = await client.api('/print/shares')
    .version('beta')
    .get();

```