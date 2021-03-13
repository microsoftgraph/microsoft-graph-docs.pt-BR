---
title: Tipo de recurso passwordSingleSignOnSettings
description: Configurações relacionadas ao login único baseado em senha
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3e7e4402e6416166dd7c288cdd9aa9ec5ecbba06
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761539"
---
# <a name="passwordsinglesignonsettings-resource-type"></a>Tipo de recurso passwordSingleSignOnSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém a coleção de configurações de login único baseada em senha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|campos|[Coleção passwordSingleSignOnField](passwordsinglesignonfield.md)||

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnSettings",
  "baseType": null
}-->

```json
{
  "fields": [{"@odata.type": "microsoft.graph.passwordSingleSignOnField"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

