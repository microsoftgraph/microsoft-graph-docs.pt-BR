---
title: Tipo de recurso userExperienceAnalyticsSettings
description: O insight de análise de experiência do usuário é a recomendação para melhorar a pontuação de análise da experiência do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67d42f2c7e42fa9ad05a83e59ab5c046b9f08af6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046929"
---
# <a name="userexperienceanalyticssettings-resource-type"></a>Tipo de recurso userExperienceAnalyticsSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O insight de análise de experiência do usuário é a recomendação para melhorar a pontuação de análise da experiência do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|configurationManagerDataConnectorConfigured|Boleano|True se a anexação de locatário estiver configurada. Se configurado, os dispositivos conectados ao locatário SCCM aparecerão no relatório UXA.|

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



