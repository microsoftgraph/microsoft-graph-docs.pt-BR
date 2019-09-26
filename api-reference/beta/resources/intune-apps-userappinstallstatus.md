---
title: tipo de recurso userAppInstallStatus
description: Contém propriedades para o status de instalação de um usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f55ecd0eff7e0367e4bd312b35210fe4e9f3bb55
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199101"
---
# <a name="userappinstallstatus-resource-type"></a>tipo de recurso userAppInstallStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o status de instalação de um usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Listar Propriedades e relações dos objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Obter userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Leia as propriedades e as relações do objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Criar userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Criar um novo objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Excluir userAppInstallStatus](../api/intune-apps-userappinstallstatus-delete.md)|Nenhum|Exclui [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[Atualizar userAppInstallStatus](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Atualiza as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|userName|Cadeia de caracteres|Nome de usuário.|
|userPrincipalName|String|Nome principal do usuário.|
|installedDeviceCount|Int32|Contagem de dispositivos instalados.|
|failedDeviceCount|Int32|Falha na contagem de dispositivos.|
|notInstalledDeviceCount|Int32|Sem contagem de dispositivos instalados.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[mobileApp](../resources/intune-shared-mobileapp.md)|O link de navegação para o aplicativo móvel.|
|deviceStatuses|coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|O estado de instalação do aplicativo em dispositivos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```



