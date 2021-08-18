---
title: tipo de recurso userExperienceAnalyticsCloudIdentityDevicesSummary
description: A análise da experiência do usuário funciona em qualquer lugar do resumo de dispositivos de identidade na nuvem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89f8f4fde6b0fc075c0f8dffe07406468cca4bfb
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259184"
---
# <a name="userexperienceanalyticscloudidentitydevicessummary-resource-type"></a>tipo de recurso userExperienceAnalyticsCloudIdentityDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A análise da experiência do usuário funciona em qualquer lugar do resumo de dispositivos de identidade na nuvem.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceWithoutCloudIdentityCount|Int32|A contagem de dispositivos que não são identidade de nuvem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary",
  "deviceWithoutCloudIdentityCount": 1024
}
```




