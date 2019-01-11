---
title: tipo de recurso de officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do inquilino.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ff75c5d73db35c5c2ff70ad3a3dc3e4509745188
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825230"
---
# <a name="officeclientcheckinstatus-resource-type"></a>tipo de recurso de officeClientCheckinStatus

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade que descreve as estatísticas de check-in do inquilino.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userPrincipalName|Cadeia de caracteres|Nome principal de usuário usando o dispositivo.|
|deviceName|Cadeia de caracteres|Nome do dispositivo tentando fazer check-in.|
|devicePlatform|Cadeia de caracteres|Plataforma de dispositivo tentando fazer check-in.|
|devicePlatformVersion|Cadeia de caracteres|Versão de plataforma do dispositivo tentando fazer check-in.|
|wasSuccessful|Booliano|Se o último check-in foi bem-sucedida.|
|userId|Cadeia de caracteres|Identificador de usuário usando o dispositivo.|
|checkinDateTime|DateTimeOffset|Último dispositivo tempo check-in em UTC.|
|errorMessage|Cadeia de caracteres|Mensagem de erro, se houver algum associado para o último check-in.|
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



