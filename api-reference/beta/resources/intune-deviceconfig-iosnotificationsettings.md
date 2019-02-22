---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2876146e7e20ad94a7356f623a5b2e17443a18f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172699"
---
# <a name="iosnotificationsettings-resource-type"></a>Tipo de recurso iosNotificationSettings

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um item que descreve a configuração de notificação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleID|String|Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.|
|appName|Cadeia de caracteres|Nome do aplicativo a ser associado à bundleID.|
|publicador|String|Publicador a ser associado à bundleID.|
|enabled|Boolean|Indica se são permitidas notificações neste aplicativo.|
|showInNotificationCenter|Booliano|Indica se as notificações podem ser exibidas no centro de notificações.|
|showOnLockScreen|Booliano|Indica se as notificações podem ser exibidas na tela de bloqueio.|
|alertType|[iosNotificationAlertType](../resources/intune-deviceconfig-iosnotificationalerttype.md)|Indica o tipo de alerta para notificações neste aplicativo. Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.|
|badgesEnabled|Booliano|Indica se serão permitidos selos neste aplicativo.|
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




