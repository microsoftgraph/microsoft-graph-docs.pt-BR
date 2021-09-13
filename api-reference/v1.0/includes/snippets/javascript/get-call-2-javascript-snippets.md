---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c15ea16ed77b1288417ee095c075836a85adc30001b6347c2572409026844ab1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let call = await client.api('/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92')
    .get();

```