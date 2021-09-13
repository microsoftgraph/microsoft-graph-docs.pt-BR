---
title: tipo de recurso userExperienceAnalyticsCloudIdentityDevicesSummary
description: A análise da experiência do usuário funciona em qualquer lugar do resumo de dispositivos de identidade na nuvem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4042ae6b67e5e5ba1ea8e493b71aeb013121227
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141139"
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



