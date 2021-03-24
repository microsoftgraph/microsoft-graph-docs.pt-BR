---
title: tipo de recurso userExperienceAnalyticsCloudManagementDevicesSummary
description: A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0fb4e7d9a8ac5b2ab9c134d45c2e625a935b491
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146744"
---
# <a name="userexperienceanalyticscloudmanagementdevicessummary-resource-type"></a>tipo de recurso userExperienceAnalyticsCloudManagementDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|coManagedDeviceCount|Int32|Número total de dispositivos co-gerenciados.|
|intuneDeviceCount|Int32|A contagem de dispositivos do intune que não estão no piloto automático registrado.|
|tenantAttachDeviceCount|Int32|Contagem total de dispositivos de anexação de locatários.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
  "coManagedDeviceCount": 1024,
  "intuneDeviceCount": 1024,
  "tenantAttachDeviceCount": 1024
}
```




