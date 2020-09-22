---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: O recurso personOrGroupColumn em uma columnDefinition indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.
doc_type: resourcePageType
ms.openlocfilehash: 8d4875ba813f5c1491135b2d1615c4146b438304
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032415"
---
# <a name="personorgroupcolumn-resource-type"></a>Tipo de recurso PersonOrGroupColumn

Namespace: microsoft.graph

O recurso **personOrGroupColumn** em uma [columnDefinition](columndefinition.md) indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **personOrGroupColumn**.
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade              | Tipo    | Descrição
|:---------------------------|:--------|:--------------------------------------
| **allowMultipleSelection** | booliano | Indica se vários valores podem ser selecionados da origem.
| **displayAs**              | string  | Como exibir as informações sobre a pessoa ou grupo escolhido. Veja a seguir.
| **chooseFromType**         | string  | Se permite somente a seleção de pessoas, ou de pessoas e grupos. Deve ser `peopleAndGroups` ou `peopleOnly`.

## <a name="displayas-options"></a>Opções de displayas

| Valor de displayAs               | Descrição
|:------------------------------|:-----------------------
| **account**                   | A cadeia de caracteres de declaração codificada bruta do SharePoint para a pessoa ou grupo (por exemplo. `i:0#.f|membership|jane@contoso.com`).
| **department**                | O departamento da pessoa ou grupo.
| **firstName**                 | O primeiro nome da pessoa.
| **id**                        | A id da pessoa ou grupo no diretório.
| **lastName**                  | O sobrenome da pessoa.
| **mobilePhone**               | O número de celular da pessoa.
| **name**                      | O nome da pessoa.
| **nameWithPictureAndDetails** | O nome da pessoa com sua imagem e detalhes adicionais.
| **nameWithPresence**          | Padrão. O nome da pessoa com um ícone indicador de presença (disponível/ocupado/etc.)
| **office**                    | O número comercial da pessoa.
| **pictureOnly36x36**          | Imagem da pessoa, delimitada por um quadrado de 36 x 36 pixels.
| **pictureOnly48x48**          | Imagem da pessoa, delimitada por um quadrado de 48 x 48 pixels.
| **pictureOnly72x72**          | Imagem da pessoa, delimitada por um quadrado de 72 x 72 pixels.
| **sipAddress**                | O endereço sip da pessoa.
| **title**                     | O cargo da pessoa na organização.
| **userName**                  | O nome de usuário da pessoa ou grupo.
| **workEmail**                 | O endereço de email da pessoa ou grupo.
| **workPhone**                 | O número de telefone comercial da pessoa.

Observação: podem ser retornados tipos adicionais de DisplayAs.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->

