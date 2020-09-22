---
title: tipo de recurso bitlockerRecoveryKey
description: Recurso de chave de recuperação do BitLocker
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 038feb77f7ca57d426a44c04b3d9c93ae29e5aa4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081943"
---
# <a name="bitlockerrecoverykey-resource-type"></a>tipo de recurso bitlockerRecoveryKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma chave BitLocker armazenada que contém a chave de recuperação real por meio da propriedade **Key** .

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar recoveryKeys](../api/bitlocker-list-recoverykeys.md)|coleção [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Obtenha uma lista dos objetos [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades.|
|[Obter bitlockerRecoveryKey](../api/bitlockerrecoverykey-get.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Recupere as propriedades e os relacionamentos de um objeto [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) . Observação: a propriedade **Key** não é retornada por padrão.|

> **Observação**: apenas algumas funções têm as permissões para chamar essas APIs.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que a chave foi originalmente convertida no Azure Active Directory.|
|deviceId|Cadeia de caracteres|ID do dispositivo do qual é feito o backup da chave BitLocker originalmente.|
|id|Cadeia de caracteres|O identificador exclusivo da chave do BitLocker.|
|chave|Cadeia de caracteres|A chave de recuperação do BitLocker.|
|volumetype|volumetype|Indica o tipo de volume ao qual a chave BitLocker está associada. Os valores possíveis são: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.|

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
  "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
  "createdDateTime": "2020-06-15T13:45:30.0000000Z",
  "volumeType": 1,
  "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
  "key": "123456-231453-873456-213546-654678-765689-123456-324565"
}
```

