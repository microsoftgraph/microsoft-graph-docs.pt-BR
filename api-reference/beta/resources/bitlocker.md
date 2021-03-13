---
title: tipo bitlocker
description: Recurso BitLocker
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3e714015b3834051371861880355360f02d12166
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761832"
---
# <a name="bitlocker-resource-type"></a>Tipo de recurso bitlocker

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso pai de uma chave BitLocker armazenada com a propriedade de navegação **bitlockerRecoveryKey** que contém a chave de recuperação real.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar recoveryKeys](../api/bitlocker-list-recoverykeys.md)|[Coleção bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Obter uma lista dos objetos bitlockerRecoveryKey e suas propriedades.|

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
| Relação | Tipo | Descrição |
|--|--|--|
| recoveryKeys | [Coleção bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) | As chaves de recuperação associadas à entidade bitlocker. |

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

