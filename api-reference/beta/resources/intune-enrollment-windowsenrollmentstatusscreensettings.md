---
title: tipo de recurso de windowsEnrollmentStatusScreenSettings
description: Configuração de tela do status de inscrição
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399931"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>tipo de recurso de windowsEnrollmentStatusScreenSettings

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Configuração de tela do status de inscrição

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hideInstallationProgress|Boolean|Mostrar ou ocultar o progresso da instalação para o usuário|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|Permitir ou bloquear um usuário utilize um dispositivo antes da instalação de perfil e o aplicativo completo|
|blockDeviceSetupRetryByUser|Boolean|Permitir que o usuário repetir a instalação em caso de falha de instalação|
|allowLogCollectionOnInstallFailure|Boolean|Permitir ou bloquear o conjunto de log em caso de falha de instalação|
|customErrorMessage|String|Definir a mensagem de erro personalizada para mostrar após a falha de instalação|
|installProgressTimeoutInMinutes|Int32|Definir tempo limite de progresso de instalação em minutos|
|allowDeviceUseOnInstallFailure|Boolean|Permitir que o usuário continue a usar o dispositivo em caso de falha de instalação|

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




