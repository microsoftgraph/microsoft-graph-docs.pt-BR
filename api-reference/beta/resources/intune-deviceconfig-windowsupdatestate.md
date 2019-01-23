---
title: tipo de recurso de windowsUpdateState
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20387d9e1fd9b84853a7bc097dfa08d128809358
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429162"
---
# <a name="windowsupdatestate-resource-type"></a>tipo de recurso de windowsUpdateState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Esta é a Id da entidade.|
|deviceId|Cadeia de caracteres|A identificação do dispositivo.|
|userId|String|A identificação do usuário.|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo.|
|userPrincipalName|String|Nome principal do usuário.|
|status|[windowsUpdateStatus] (.. /Resources/Intune-deviceconfig-windowsupdatestatus.MD)|Status de udpate do Windows.|
|qualityUpdateVersion|String|A versão de atualização de qualidade do dispositivo.|
|featureUpdateVersion|String|A versão atual de atualização do recurso do dispositivo.|
|lastScanDateTime|DateTimeOffset|A data de tempo que o Windows Update Agent foi uma verificação bem-sucedida.|
|lastSyncDateTime|DateTimeOffset|Última data e hora em que o dispositivo é sincronizado com o Microsoft Intune.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.WindowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.WindowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String (identifier)",
  "userId": "String (identifier)",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```


