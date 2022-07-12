---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 014198d37e028b0705d035688a004ea6b0ab84d4
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734757"
---
# <a name="iosnotificationsettings-resource-type"></a>Tipo de recurso iosNotificationSettings

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um item que descreve a configuração de notificação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleID|Cadeia de caracteres|Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.|
|appName|Cadeia de caracteres|Nome do aplicativo a ser associado à bundleID.|
|publicador|Cadeia de caracteres|Publicador a ser associado à bundleID.|
|enabled|Booliano|Indica se são permitidas notificações neste aplicativo.|
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





