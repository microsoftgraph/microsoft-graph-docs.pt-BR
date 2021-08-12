---
title: Tipo de recurso printSettings
description: Representa as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4174f6f8dbd1a94ce3246189683529a9fdb4346927465b3f084fb77974313992
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163751"
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

