---
title: tipo de recurso relatedContact
description: Representa um registro de contato relacionado a um educationUser que fornece informações para tutores, auxiliares, médicos e assim por diante.
author: marcla
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5d833afe05480a1ae4e490220ad16755f268c7a
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589433"
---
# <a name="relatedcontact-resource-type"></a>tipo de recurso relatedContact

Namespace: microsoft.graph

Representa um registro de contato relacionado a [um educationUser](../resources/educationuser.md) que fornece informações para tutores, auxiliares, médicos e assim por diante.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                  | Descrição                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| accessConsent | Booliano               | Indica se o usuário foi consentido para acessar dados de alunos.                                                                     |
| displayName   | Cadeia de caracteres                | Nome do contato. Obrigatório.                                                                                                            |
| emailAddress  | String                | Endereço de email principal do contato. Obrigatório.                                                                                           |
| mobilePhone   | String                | Número de telefone celular do contato.                                                                                                       |
| relação  | contactRelationship | Relação com o usuário. Os valores possíveis são: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "accessConsent": true,
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String"
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
