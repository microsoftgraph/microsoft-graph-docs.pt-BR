---
title: Tipo de recurso windowsEnrollmentStatusScreenSettings
description: Configuração da tela de status do registro
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f483d4217506aa440df1108c968ba4df83f8fc7f55433e193d4c07388a70ce2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164213"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Tipo de recurso windowsEnrollmentStatusScreenSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração da tela de status do registro

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hideInstallationProgress|Boolean|Mostrar ou ocultar o progresso da instalação para o usuário|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|Permitir ou bloquear o usuário para usar o dispositivo antes da conclusão da instalação do perfil e do aplicativo|
|blockDeviceSetupRetryByUser|Boolean|Permitir que o usuário repetir a instalação na falha de instalação|
|allowLogCollectionOnInstallFailure|Boolean|Permitir ou bloquear o conjunto de log na falha de instalação|
|customErrorMessage|Cadeia de caracteres|Definir mensagem de erro personalizada para mostrar após a falha na instalação|
|installProgressTimeoutInMinutes|Int32|Definir o tempo de tempo de duração da instalação em minutos|
|allowDeviceUseOnInstallFailure|Boolean|Permitir que o usuário continue usando o dispositivo na falha de instalação|

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




