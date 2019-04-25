---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9806c1d263710ecaef2c04af89926e7568ad94da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566413"
---
# <a name="organization-resource-type"></a>tipo de recurso organization

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar organizações](../api/intune-onboarding-organization-list.md)|Coleção [organization](../resources/intune-onboarding-organization.md)|Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).|
|[Obter organização](../api/intune-onboarding-organization-get.md)|[organization](../resources/intune-onboarding-organization.md)|Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).|
|[Atualizar a organização](../api/intune-onboarding-organization-update.md)|[organização](../resources/intune-onboarding-organization.md)|Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).|
|[Ação setMobileDeviceManagementAuthority](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|Int32|Define a autoridade de gerenciamento de dispositivo móvel|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto.|
|mobileDeviceManagementAuthority|[mdmAuthority](../resources/intune-onboarding-mdmauthority.md)|Define autoridade de gerenciamento de dispositivo móvel. Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.|
|certificateConnectorSetting|[certificateConnectorSetting](../resources/intune-onboarding-certificateconnectorsetting.md)|Configuração do conector de certificado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```





