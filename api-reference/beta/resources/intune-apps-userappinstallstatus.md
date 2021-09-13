---
title: Tipo de recurso userAppInstallStatus
description: Contém propriedades para o status de instalação de um usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee0488490b022d7a1e26ac532cac4613d0d06b1c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047167"
---
# <a name="userappinstallstatus-resource-type"></a>Tipo de recurso userAppInstallStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o status de instalação de um usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|[Coleção userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Listar propriedades e relações dos [objetos userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)|
|[Obter userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Leia propriedades e relações do [objeto userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)|
|[Criar userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Crie um novo [objeto userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)|
|[Excluir userAppInstallStatus](../api/intune-apps-userappinstallstatus-delete.md)|Nenhum|Exclui um [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[Atualizar userAppInstallStatus](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Atualize as propriedades de um [objeto userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userName|Cadeia de caracteres|Nome de usuário.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário.|
|installedDeviceCount|Int32|Contagem de dispositivos instalados.|
|failedDeviceCount|Int32|Falha na contagem de dispositivos.|
|notInstalledDeviceCount|Int32|Sem contagem de dispositivos instalados.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[mobileApp](../resources/intune-shared-mobileapp.md)|O link de navegação para o aplicativo móvel.|
|deviceStatuses|[Coleção mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|O estado de instalação do aplicativo em dispositivos.|

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



