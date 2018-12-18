---
title: tipo de recurso de userAppInstallStatus
description: Contém propriedades para o status de instalação de um usuário.
author: tfitzmac
ms.openlocfilehash: 024fff32aac2a268a2e0bbec81a6d46b31012a11
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302755"
---
# <a name="userappinstallstatus-resource-type"></a>tipo de recurso de userAppInstallStatus

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades para o status de instalação de um usuário.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Lista as propriedades e os relacionamentos dos objetos [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Obter userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Leia as propriedades e os relacionamentos do objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Criar userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Crie um novo objeto de [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Excluir userAppInstallStatus](../api/intune-apps-userappinstallstatus-delete.md)|Nenhum|Exclui um [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[Atualizar userAppInstallStatus](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Atualize as propriedades de um objeto [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|userName|Cadeia de caracteres|Nome de usuário.|
|userPrincipalName|String|Nome Principal de usuário.|
|installedDeviceCount|Int32|Contagem de dispositivos instalados.|
|failedDeviceCount|Int32|Falha na contagem de dispositivos.|
|notInstalledDeviceCount|Int32|Sem contagem de dispositivos instalados.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|app|[mobileApp](../resources/intune-apps-mobileapp.md)|O link de navegação para o aplicativo móvel.|
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





