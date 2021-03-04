---
title: Tipo de recurso bitlockerRecoveryKey
description: Recurso de chave de recuperação do BitLocker
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 466a5d907b3deb589ec1b70351903e24aba0ab32
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443150"
---
# <a name="bitlockerrecoverykey-resource-type"></a>Tipo de recurso bitlockerRecoveryKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma chave BitLocker armazenada que contém a chave de recuperação real por meio da **propriedade key.**

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar recoveryKeys](../api/bitlocker-list-recoverykeys.md)|[Coleção bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Obter uma lista dos [objetos bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades.|
|[Obter bitlockerRecoveryKey](../api/bitlockerrecoverykey-get.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Recupere as propriedades e as relações de um [objeto bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md) Observação: a **propriedade key** não é retornada por padrão.|

> **Observação**: apenas algumas funções têm as permissões para chamar essas APIs.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que a chave foi originalmente respaldada no Azure Active Directory.|
|deviceId|Cadeia de caracteres|ID do dispositivo de onde a chave BitLocker é originalmente respaldada.|
|id|String|O identificador exclusivo da chave BitLocker.|
|chave|String|A chave de recuperação BitLocker.|
|volumeType|volumeType|Indica o tipo de volume ao qual a chave BitLocker está associada. Os valores possíveis são: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.|

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

