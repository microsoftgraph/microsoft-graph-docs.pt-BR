---
title: Tipo de recurso userExperienceAnalyticsSettings
description: O insight de análise de experiência do usuário é a recomendação para melhorar a pontuação de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 877e710d00405f3b9a592cd7eb2501d25495d0a61237ea5acc62f6cb9e4f38d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185681"
---
# <a name="userexperienceanalyticssettings-resource-type"></a>Tipo de recurso userExperienceAnalyticsSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O insight de análise de experiência do usuário é a recomendação para melhorar a pontuação de análise da experiência do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|configurationManagerDataConnectorConfigured|Boolean|True se a anexação de locatário estiver configurada. Se configurado, os dispositivos conectados ao locatário SCCM aparecerão no relatório UXA.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsSettings",
  "configurationManagerDataConnectorConfigured": true
}
```




