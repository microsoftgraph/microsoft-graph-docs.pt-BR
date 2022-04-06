---
title: Tipo de recurso cloudPcWindowsSettings
description: Representa configurações Windows específicas a ser configuradas durante a criação de PCs na Nuvem para uma política de provisionamento.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3a58fe434e73402f9d69902c58da5f20f78c5a89
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722622"
---
# <a name="cloudpcwindowssettings-resource-type"></a>Tipo de recurso cloudPcWindowsSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações Windows específicas a ser configuradas durante a criação de PCs na Nuvem para uma política de provisionamento.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|idioma|Cadeia de caracteres|A Windows de idioma/região a ser usada para configuração e localização do pacote de idiomas do Cloud PC. O valor padrão é `en-US`, que corresponde ao inglês (Estados Unidos).|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcWindowsSettings",
  "language": "String"
}
```
