---
title: tipo de recurso de officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do inquilino.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a387e04b9ebc15d65eb8dd883ecd4a9bae78ad6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969286"
---
# <a name="officeclientcheckinstatus-resource-type"></a>tipo de recurso de officeClientCheckinStatus

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade que descreve as estatísticas de check-in do inquilino.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userPrincipalName|String|Nome principal de usuário usando o dispositivo.|
|deviceName|String|Nome do dispositivo tentando fazer check-in.|
|devicePlatform|String|Plataforma de dispositivo tentando fazer check-in.|
|devicePlatformVersion|String|Versão de plataforma do dispositivo tentando fazer check-in.|
|wasSuccessful|Booliano|Se o último check-in foi bem-sucedida.|
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



