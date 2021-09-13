---
title: Tipo de recurso windowsEnrollmentStatusScreenSettings
description: Configuração da tela de status do registro
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f7578f25bf3ed2ed8b47d6cb7c039fd6bda7b89a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039893"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Tipo de recurso windowsEnrollmentStatusScreenSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração da tela de status do registro

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|hideInstallationProgress|Boleano|Mostrar ou ocultar o progresso da instalação para o usuário|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boleano|Permitir ou bloquear o usuário para usar o dispositivo antes da conclusão da instalação do perfil e do aplicativo|
|blockDeviceSetupRetryByUser|Boleano|Permitir que o usuário repetir a instalação na falha de instalação|
|allowLogCollectionOnInstallFailure|Boleano|Permitir ou bloquear o conjunto de log na falha de instalação|
|customErrorMessage|Cadeia de Caracteres|Definir mensagem de erro personalizada para mostrar após a falha na instalação|
|installProgressTimeoutInMinutes|Int32|Definir o tempo de tempo de duração da instalação em minutos|
|allowDeviceUseOnInstallFailure|Boleano|Permitir que o usuário continue usando o dispositivo na falha de instalação|

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



