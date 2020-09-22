---
title: tipo de BitLocker
description: Recurso do BitLocker
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ad8a05e82cd3f300bedf034fe18f67ce3359f16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038862"
---
# <a name="bitlocker-resource-type"></a>tipo de recurso do BitLocker

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso pai de uma chave do BitLocker armazenada com a propriedade de navegação **bitlockerRecoveryKey** que contém a chave de recuperação real.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar recoveryKeys](../api/bitlocker-list-recoverykeys.md)|coleção [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Obtenha uma lista dos objetos bitlockerRecoveryKey e suas propriedades.|

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
| Relação | Tipo | Descrição |
|--|--|--|
| recoveryKeys | coleção [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) | As chaves de recuperação associadas à entidade do BitLocker. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitlocker",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlocker"
}
```

