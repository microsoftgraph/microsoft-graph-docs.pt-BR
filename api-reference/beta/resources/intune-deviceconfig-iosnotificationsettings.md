---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: tfitzmac
ms.openlocfilehash: c24e0719e634d2939f88280431538b41fb0a1b5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359189"
---
# <a name="iosnotificationsettings-resource-type"></a>Tipo de recurso iosNotificationSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





