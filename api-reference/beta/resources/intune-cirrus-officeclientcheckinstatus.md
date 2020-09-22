---
title: tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 647d55e3d5eca6acb47b90092dc0502097b63cf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021760"
---
# <a name="officeclientcheckinstatus-resource-type"></a>tipo de recurso officeClientCheckinStatus

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que descreve as estatísticas de check-in do locatário.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userPrincipalName|String|Nome principal do usuário usando o dispositivo.|
|deviceName|String|Nome do dispositivo que está tentando fazer check-in.|
|devicePlatform|String|Plataforma do dispositivo que está tentando fazer check-in.|
|devicePlatformVersion|String|Versão da plataforma do dispositivo que está tentando fazer check-in.|
|wasSuccessful|Booliano|Se o último check-in foi bem-sucedido.|
|userId|Cadeia de caracteres|Identificador de usuário usando o dispositivo.|
|checkinDateTime|DateTimeOffset|Tempo de check-in do último dispositivo em UTC.|
|errorMessage|String|Mensagem de erro se algum associado para o último check-in.|
|appliedPolicies|Coleção String|Lista de políticas entregues ao dispositivo como última verificação.|

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






