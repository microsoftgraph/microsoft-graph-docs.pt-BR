---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33cde8451b13155a8d2c3c2e1a24af8053e26cc2bac2dd973ae51b11f0a3eb22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216643"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAsset updatableAsset = graphClient.admin().windows().updates().updatableAssets("5c55730b-730b-5c55-0b73-555c0b73555c")
    .buildRequest()
    .get();

```