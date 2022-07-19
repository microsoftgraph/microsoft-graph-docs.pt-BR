---
title: Tipo de recurso submissionDetectedFile
description: Representa as informações de um arquivo detectado em um envio de ameaça
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5d12212968b55125776831b770f93b1e482162b3
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856521"
---
# <a name="submissiondetectedfile-resource-type"></a>Tipo de recurso submissionDetectedFile

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de um arquivo detectado em um envio de ameaça.

## <a name="properties"></a>Propriedades
| Propriedade | Tipo   | Descrição    |
|:---------|:-------|:---------------|
| fileHash | Cadeia de caracteres | O hash do arquivo. |
| fileName | String | O nome do arquivo. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionDetectedFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionDetectedFile",
  "fileName": "String",
  "fileHash": "String"
}
```

