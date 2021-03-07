---
title: Tipo de recurso printSettings
description: Representa as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 53e0db2a1923cad0af1f35baf5bed6fecd896fb3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516861"
---
# <a name="printsettings-resource-type"></a>Tipo de recurso printSettings

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa as configurações de todo o locatário para o serviço de Impressão Universal.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|documentConversionEnabled|Booliano|Especifica se a conversão de documento está habilitada para o locatário. Se a conversão de documentos estiver habilitada, o serviço de Impressão Universal converterá automaticamente documentos em um formato compatível com a impressora (xps para pdf) quando necessário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printSettings",
  "documentConversionEnabled": "Boolean"
}
```

