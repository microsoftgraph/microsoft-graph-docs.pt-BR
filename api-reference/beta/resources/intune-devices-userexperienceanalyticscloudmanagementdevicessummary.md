---
title: tipo de recurso userExperienceAnalyticsCloudManagementDevicesSummary
description: A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed76d8c2c4c26c6ba010bd21829a70f014538937
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803760"
---
# <a name="userexperienceanalyticscloudmanagementdevicessummary-resource-type"></a>tipo de recurso userExperienceAnalyticsCloudManagementDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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



