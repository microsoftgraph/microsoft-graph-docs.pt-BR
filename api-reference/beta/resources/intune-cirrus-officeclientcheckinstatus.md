---
title: tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df8f1927329a34a51b5f6d8738faec05be01b451
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011999"
---
# <a name="officeclientcheckinstatus-resource-type"></a>tipo de recurso officeClientCheckinStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que descreve as estatísticas de check-in do locatário.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userPrincipalName|String|Nome principal do usuário usando o dispositivo.|
|deviceName|String|Nome do dispositivo que está tentando fazer check-in.|
|devicePlatform|String|Plataforma do dispositivo que está tentando fazer check-in.|
|devicePlatformVersion|String|Versão da plataforma do dispositivo que está tentando fazer check-in.|
|wasSuccessful|Booliano|Se o último check-in foi bem-sucedido.|
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



