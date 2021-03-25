---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 744cf49083aa9091e1e3a5286db8244cf6870e46
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209656"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableCollectionPage tables = graphClient.me().drive().items("{id}").workbook().tables()
    .buildRequest()
    .get();

```