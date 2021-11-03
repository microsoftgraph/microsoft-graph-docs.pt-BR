---
title: recurso bitLocker
description: O recurso pai de uma chave BitLocker armazenada com a propriedade de navegação bitlockerRecoveryKey que contém a chave de recuperação real.
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ac73c0e7237f4d41217cb53c2c4c33d8cfcdb784
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689071"
---
# <a name="bitlocker-resource-type"></a>Tipo de recurso bitlocker

Namespace: microsoft.graph

O recurso pai de uma chave BitLocker armazenada com a propriedade de navegação **bitlockerRecoveryKey** que contém a chave de recuperação real.

## <a name="methods"></a>Métodos
Nenhum.

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

