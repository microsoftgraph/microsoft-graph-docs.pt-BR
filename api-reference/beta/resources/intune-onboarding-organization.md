---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
ms.openlocfilehash: e7e49e5676e412ea0e174b2e158b98efea8e0c7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036779"
---
# <a name="organization-resource-type"></a>tipo de recurso organization

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar organizações](../api/intune-onboarding-organization-list.md)|Coleção [organization](../resources/intune-onboarding-organization.md)|Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).|
|[Obter organização](../api/intune-onboarding-organization-get.md)|[organização](../resources/intune-onboarding-organization.md)|Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).|
|[Atualizar a organização](../api/intune-onboarding-organization-update.md)|[organização](../resources/intune-onboarding-organization.md)|Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).|
|[Ação setMobileDeviceManagementAuthority](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|Int32|Define a autoridade de gerenciamento de dispositivo móvel|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
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





