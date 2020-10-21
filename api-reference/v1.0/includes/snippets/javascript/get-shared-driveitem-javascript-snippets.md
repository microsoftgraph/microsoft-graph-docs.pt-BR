---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f239c56fed4b7324fb4249c3f4d87233b60868d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .get();

```