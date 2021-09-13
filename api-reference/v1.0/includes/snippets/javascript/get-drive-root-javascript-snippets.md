---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a841acdae5f3f29e7412c47f1d107ca641aadbb27c2eb7722bf4653cd00a5a52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/me/drive/root')
    .get();

```