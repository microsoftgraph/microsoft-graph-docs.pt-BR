---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b69112830e9feba3ff2c708b7028e106c0aadb09175d517129f975fb8870afcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327481"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organization = await client.api('/organization')
    .get();

```