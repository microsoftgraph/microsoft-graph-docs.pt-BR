---
title: tipo de recurso implicitGrantSettings
description: Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microasoft-identity-platform
author: sureshja
ms.openlocfilehash: a01abc5d0c3937b6c95353ed0aa425eeb9dbc33d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466410"
---
# <a name="implicitgrantsettings-resource-type"></a>tipo de recurso implicitGrantSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Booliano | Especifica se este aplicativo Web pode solicitar um token de ID usando o fluxo implícito do OAuth 2,0.|
|enableAccessTokenIssuance| Booliano | Especifica se este aplicativo Web pode solicitar um token de acesso usando o fluxo implícito do OAuth 2,0.|

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
