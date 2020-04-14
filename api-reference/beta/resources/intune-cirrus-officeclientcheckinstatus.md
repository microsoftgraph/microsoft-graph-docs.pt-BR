---
title: tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a2f8bb8728a43187903016ca3417b8e6655b3ab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471486"
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



