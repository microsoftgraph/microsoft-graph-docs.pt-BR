---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c748c0ba5d21674438af0c7a60883ab8c9832e09
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790570"
---
# <a name="iosnotificationsettings-resource-type"></a>Tipo de recurso iosNotificationSettings

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um item que descreve a configuração de notificação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleID|String|Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.|
|appName|Cadeia de caracteres|Nome do aplicativo a ser associado à bundleID.|
|publicador|String|Publicador a ser associado à bundleID.|
|enabled|Boolean|Indica se são permitidas notificações neste aplicativo.|
|showInNotificationCenter|Boolean|Indica se as notificações podem ser exibidas no centro de notificações.|
|showOnLockScreen|Boolean|Indica se as notificações podem ser exibidas na tela de bloqueio.|
|alertType|[iosNotificationAlertType](../resources/intune-deviceconfig-iosnotificationalerttype.md)|Indica o tipo de alerta para notificações neste aplicativo. Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.|
|badgesEnabled|Boolean|Indica se serão permitidos selos neste aplicativo.|
|soundsEnabled|Booliano|Indica se são permitidos sons neste aplicativo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



