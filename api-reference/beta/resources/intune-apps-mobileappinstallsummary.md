---
title: tipo de recurso mobileAppInstallSummary
description: Contém propriedades para o resumo de instalação de um aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a981477daefae92b6afcd3612a173d75b37e8637
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551866"
---
# <a name="mobileappinstallsummary-resource-type"></a>tipo de recurso mobileAppInstallSummary

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de instalação de um aplicativo móvel.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Leia as propriedades e as relações do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .|
|[Atualizar mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Atualiza as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|installedDeviceCount|Int32|Número de dispositivos que instalaram com êxito este aplicativo.|
|failedDeviceCount|Int32|Número de dispositivos que falharam ao instalar este aplicativo.|
|notApplicableDeviceCount|Int32|Número de dispositivos que não se aplicam a este aplicativo.|
|notInstalledDeviceCount|Int32|Número de dispositivos que não possuem este aplicativo instalado.|
|pendingInstallDeviceCount|Int32|Número de dispositivos que foram notificados para instalar este aplicativo.|
|installedUserCount|Int32|Número de usuários cujos dispositivos foram todos bem-sucedidos para instalar este aplicativo.|
|failedUserCount|Int32|Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.|
|notApplicableUserCount|Int32|Número de usuários cujos dispositivos não são todos aplicáveis para este aplicativo.|
|notInstalledUserCount|Int32|Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.|
|pendingInstallUserCount|Int32|Número de usuários que têm um ou mais dispositivos que foram notificados para instalar este aplicativo e têm 0 dispositivos com falhas.|

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





