---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e122145017ae3700e6df8b7d1c9f3ab361f32c269d322071db8e4bc15b3248f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applications = await client.api('/applications')
    .get();

```