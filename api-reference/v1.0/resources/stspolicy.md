---
title: Tipo de recurso stsPolicy
description: Representa um tipo de base abstrato para tipos de política que controlam plataforma de identidade da Microsoft comportamento.
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04ab6b06bbe099759802a57b6bbfdc337a233ef6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59122961"
---
# <a name="stspolicy-resource-type"></a>Tipo de recurso stsPolicy

Namespace: microsoft.graph

Representa um tipo de base abstrato para tipos de política que controlam [plataforma de identidade da Microsoft](/azure/active-directory/develop/) comportamento.

Herda de [policyBase](policyBase.md).

## <a name="methods"></a>Métodos

Nenhum(a)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo dessa política. Somente leitura. Herdado de [policyBase](policyBase.md).|
|description|String| Descrição dessa política. Herdado de [policyBase](policyBase.md).|
|displayName|Cadeia de caracteres| Nome de exibição para esta política. Herdado de [policyBase](policyBase.md).|
|definition|Coleção String| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações de uma política. A sintaxe da definição difere para cada tipo de política derivado. Obrigatório.|
|isOrganizationDefault|Booliano|Se definido como true, ativa essa política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização. Opcional, o valor padrão é false.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stsPolicy",
  "baseType": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": ["String"],
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
