---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b94c1addaa470e4b3ecf2b48f6468a97e74bae6340280adc20c85347fe52ea1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .get();

```