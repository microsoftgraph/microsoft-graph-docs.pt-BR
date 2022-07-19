---
title: Tipo de recurso submissionAdminReview
description: Representa informações de revisão do administrador para envio de ameaças
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 410ffc88cb5d5fade44456b928996834c7722cac
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856505"
---
# <a name="submissionadminreview-resource-type"></a>Tipo de recurso submissionAdminReview

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações de revisão do administrador para um envio de ameaças. Atualmente, há suporte para apenas um envio de ameaça de email relatado pelo usuário e pode ser revisado por um administrador.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo                     | Descrição                                  |
|:---------------|:-------------------------|:---------------------------------------------|
| reviewBy       | Cadeia de caracteres                   | Especifica quem examinou o email. A identificação é uma ID de email ou outras cadeias de caracteres de identidade.|
| reviewDateTime | DateTimeOffset           | Especifica a data em que a revisão ocorreu.|
| reviewResult   | submissionResultCategory | Especifica qual foi o resultado da revisão. Os valores possíveis são: , , , , , `allowedByPolicy`, `blockedByPolicy`, `spoof`, `unknown`, `noResultAvailable`e `unknownFutureValue`. `malware``phishing``spam``notJunk`  |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionAdminReview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionAdminReview",
  "reviewDateTime": "String (timestamp)",
  "reviewResult": "String",
  "reviewBy": "String"
}
```

