---
title: Tipo de recurso implicitGrantSettings
description: 'Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fe471eefe817e48468258195dae4c93331dd6e04
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547012"
---
# <a name="implicitgrantsettings-resource-type"></a>Tipo de recurso implicitGrantSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica se esse aplicativo Web pode solicitar tokens usando o fluxo implícito OAuth 2.0. Propriedades separadas estão disponíveis para solicitar ID e acessar tokens como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das seguintes propriedades deve ser definida como true.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Booliano | Especifica se esse aplicativo Web pode solicitar um token de ID usando o fluxo implícito OAuth 2.0.|
|enableAccessTokenIssuance| Booliano | Especifica se esse aplicativo Web pode solicitar um token de acesso usando o fluxo implícito OAuth 2.0.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```


