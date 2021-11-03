---
title: Tipo de recurso bitlockerRecoveryKey
description: Recurso de chave de recuperação do BitLocker
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8805b8cd633558145787f6a3c4f941fcabad0c62
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696137"
---
# <a name="bitlockerrecoverykey-resource-type"></a>Tipo de recurso bitlockerRecoveryKey

Namespace: microsoft.graph

Representa uma chave BitLocker armazenada que contém a chave de recuperação real por meio da **propriedade key.**

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar recoveryKeys](../api/bitlocker-list-recoverykeys.md)|[Coleção bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Obter uma lista dos [objetos bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades.|
|[Obter bitlockerRecoveryKey](../api/bitlockerrecoverykey-get.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Recupere as propriedades e as relações de um [objeto bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md) Observação: a **propriedade key** não é retornada por padrão.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que a chave foi originalmente respaldada para Azure Active Directory. Não anulável.|
|deviceId|Cadeia de caracteres|Identificador do dispositivo de onde a chave BitLocker é originalmente respaldada. Suporta `$filter` (`eq`).|
|id|String|O identificador exclusivo da chave BitLocker.|
|chave|String|A chave de recuperação BitLocker. Retornado apenas em `$select`. Não anulável.|
|volumeType|volumeType|Indica o tipo de volume ao qual a chave BitLocker está associada. Os valores possíveis são: `1` (para `operatingSystemVolume` ), `2` (para `fixedDataVolume` ), `3` (para ) e `removableDataVolume` `4` (para `unknownFutureValue` ).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "volumeType": "String",
  "deviceId": "String",
  "key": "String"
}
```

