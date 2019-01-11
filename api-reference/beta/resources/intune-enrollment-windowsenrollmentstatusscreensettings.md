---
title: tipo de recurso de windowsEnrollmentStatusScreenSettings
description: Configuração de tela do status de inscrição
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7263fdd8ab3d9a39d5081322c62cfcf76a4c7aa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877445"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>tipo de recurso de windowsEnrollmentStatusScreenSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração de tela do status de inscrição
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hideInstallationProgress|Booliano|Mostrar ou ocultar o progresso da instalação para o usuário|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Booliano|Permitir ou bloquear um usuário utilize um dispositivo antes da instalação de perfil e o aplicativo completo|
|blockDeviceSetupRetryByUser|Booliano|Permitir que o usuário repetir a instalação em caso de falha de instalação|
|allowLogCollectionOnInstallFailure|Booliano|Permitir ou bloquear o conjunto de log em caso de falha de instalação|
|customErrorMessage|Cadeia de caracteres|Definir a mensagem de erro personalizada para mostrar após a falha de instalação|
|installProgressTimeoutInMinutes|Int32|Definir tempo limite de progresso de instalação em minutos|
|allowDeviceUseOnInstallFailure|Booliano|Permitir que o usuário continue a usar o dispositivo em caso de falha de instalação|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```





