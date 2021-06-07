---
title: Tipo de recurso officeConfiguration
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20e86afa8d0d5fddf5b87a6c6667e2e16baa391a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752829"
---
# <a name="officeconfiguration-resource-type"></a>Tipo de recurso officeConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|Obter officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Leia propriedades e relações do [objeto officeConfiguration.](../resources/intune-cirrus-officeconfiguration.md)|
|Atualizar officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Atualize as propriedades de um [objeto officeConfiguration.](../resources/intune-cirrus-officeconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID da configuração do office.|
|tenantCheckinStatuses|[Coleção officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)|Lista de status de check-in do cliente do office.|
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Entidade que descreve as estatuetas de check-in do locatário|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|clientConfigurations|[Coleção officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Lista de configuração do cliente do office.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```




