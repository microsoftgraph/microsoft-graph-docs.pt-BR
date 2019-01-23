---
title: tipo de recurso de officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do inquilino.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403256"
---
# <a name="officeclientcheckinstatus-resource-type"></a>tipo de recurso de officeClientCheckinStatus

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Entidade que descreve as estatísticas de check-in do inquilino.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userPrincipalName|String|Nome principal de usuário usando o dispositivo.|
|deviceName|String|Nome do dispositivo tentando fazer check-in.|
|devicePlatform|String|Plataforma de dispositivo tentando fazer check-in.|
|devicePlatformVersion|String|Versão de plataforma do dispositivo tentando fazer check-in.|
|wasSuccessful|Boolean|Se o último check-in foi bem-sucedida.|
|userId|String|Identificador de usuário usando o dispositivo.|
|checkinDateTime|DateTimeOffset|Último dispositivo tempo check-in em UTC.|
|errorMessage|String|Mensagem de erro, se houver algum associado para o último check-in.|
|appliedPolicies|String collection|Lista de políticas entregues ao dispositivo como último check-in.|

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



