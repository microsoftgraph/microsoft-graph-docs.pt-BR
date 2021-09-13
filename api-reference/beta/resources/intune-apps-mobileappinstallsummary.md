---
title: Tipo de recurso mobileAppInstallSummary
description: Contém propriedades para o resumo de instalação de um aplicativo móvel.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1cc168933bad8a1eef5e177cc5361dd196c31cb5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124228"
---
# <a name="mobileappinstallsummary-resource-type"></a>Tipo de recurso mobileAppInstallSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de instalação de um aplicativo móvel.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Leia propriedades e relações do [objeto mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)|
|[Atualizar mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Atualize as propriedades de um [objeto mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|installedDeviceCount|Int32|Número de dispositivos que instalaram com êxito este aplicativo.|
|failedDeviceCount|Int32|Número de dispositivos que falharam ao instalar esse aplicativo.|
|notApplicableDeviceCount|Int32|Número de dispositivos que não são aplicáveis para este aplicativo.|
|notInstalledDeviceCount|Int32|Número de dispositivos que não têm esse aplicativo instalado.|
|pendingInstallDeviceCount|Int32|Número de dispositivos que foram notificados para instalar este aplicativo.|
|installedUserCount|Int32|Número de usuários cujos dispositivos foram todos bem-sucedidos para instalar este aplicativo.|
|failedUserCount|Int32|Número de usuários que têm 1 ou mais dispositivos que falharam ao instalar esse aplicativo.|
|notApplicableUserCount|Int32|Número de usuários cujos dispositivos não eram aplicáveis para este aplicativo.|
|notInstalledUserCount|Int32|Número de usuários que têm 1 ou mais dispositivos que não instalaram esse aplicativo.|
|pendingInstallUserCount|Int32|Número de usuários que têm 1 ou mais dispositivos que foram notificados para instalar esse aplicativo e têm 0 dispositivos com falhas.|

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



