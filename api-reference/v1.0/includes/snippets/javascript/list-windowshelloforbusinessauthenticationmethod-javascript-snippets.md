---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b02bd4f9d32d3685bc9c9d3c873723824da480b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsHelloForBusinessMethods = await client.api('/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods')
    .get();

```