---
title: tipo de recurso de mobileAppInstallSummary
description: Contém propriedades para o resumo da instalação de um aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a75dba8303d254aff911cc66931d52abb8b76c07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916023"
---
# <a name="mobileappinstallsummary-resource-type"></a>tipo de recurso de mobileAppInstallSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades para o resumo da instalação de um aplicativo móvel.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Leia as propriedades e os relacionamentos do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .|
|[Atualizar mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Atualize as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|installedDeviceCount|Int32|Número de dispositivos que instalou com sucesso deste aplicativo.|
|failedDeviceCount|Int32|Número de dispositivos que não tenha conseguido instalar esse aplicativo.|
|notApplicableDeviceCount|Int32|Número de dispositivos que não são aplicáveis para esse aplicativo.|
|notInstalledDeviceCount|Int32|Número de dispositivos que não tem este aplicativo instalado.|
|pendingInstallDeviceCount|Int32|Número de dispositivos que foram notificados para instalar esse aplicativo.|
|installedUserCount|Int32|Número de usuários cujos dispositivos tiveram êxito para instalar esse aplicativo.|
|failedUserCount|Int32|Número de usuários que têm 1 ou mais dispositivo com falha para instalar esse aplicativo.|
|notApplicableUserCount|Int32|Número de usuários cujos dispositivos tudo não eram aplicáveis para esse aplicativo.|
|notInstalledUserCount|Int32|Número de usuários que têm 1 ou mais dispositivos que não tiver instalado esse aplicativo.|
|pendingInstallUserCount|Int32|Número de usuários que têm 1 ou mais dispositivo que foram notificados para instalar esse aplicativo e tiver 0 dispositivos com falhas.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```





