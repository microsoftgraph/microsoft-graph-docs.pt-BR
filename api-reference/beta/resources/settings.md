---
title: tipo de recurso de configurações
description: As configurações atuais necessárias para um usuário usar a API de análise.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 822ac02be4f3dc5d507aa5d9dbbb2fa22b194b64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033530"
---
# <a name="settings-resource-type"></a>tipo de recurso de configurações

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações atuais necessárias para que um usuário use a API de análise.

Para a API de análise retornar resultados para os usuários, eles devem ter uma caixa de correio hospedada na nuvem habilitada para o Microsoft Graph, ter uma licença válida do myAnalytics e ser optou por usar myAnalytics.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
[Obter configurações](../api/useranalytics-get-settings.md) | [configurações](settings.md) | Obter as configurações de propriedade a seguir para um usuário.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hasGraphMailbox|Booliano|Especifica se a caixa de correio principal do usuário está hospedada na nuvem e está habilitada para o Microsoft Graph.|
|hasLicense|Booliano|Especifica se o usuário tem uma licença myAnalytics atribuída.|
|hasOptedOut|Booliano|Especifica se o usuário optou por ter o myAnalytics.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settings",
  "baseType": null
}-->

```json
{
  "hasGraphMailbox": true,
  "hasLicense": true,
  "hasOptedOut": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

