---
title: tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 465b07ba286b9ee3a58132424be2a25b1c7e564e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156053"
---
# <a name="officeclientcheckinstatus-resource-type"></a>tipo de recurso officeClientCheckinStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que descreve as estatísticas de check-in do locatário.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userPrincipalName|String|Nome principal do usuário usando o dispositivo.|
|deviceName|Cadeia de caracteres|Nome do dispositivo que está tentando fazer check-in.|
|devicePlatform|String|Plataforma do dispositivo que está tentando fazer check-in.|
|devicePlatformVersion|String|Versão da plataforma do dispositivo que está tentando fazer check-in.|
|wasSuccessful|Boolean|Se o último check-in foi bem-sucedido.|
|userId|String|Identificador de usuário usando o dispositivo.|
|checkinDateTime|DateTimeOffset|Tempo de check-in do último dispositivo em UTC.|
|errorMessage|String|Mensagem de erro se algum associado para o último check-in.|
|appliedPolicies|Coleção de cadeias de caracteres|Lista de políticas entregues ao dispositivo como última verificação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



