---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 715c6ca22957cbd951784e6cf32edf2bf47f1098
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="personorgroupcolumn-resource-type"></a>Tipo de recurso PersonOrGroupColumn

O recurso **personOrGroupColumn** em uma [columnDefinition](columnDefinition.md) indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.

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

## <a name="displayas-values"></a>Valores de displayAs

| Valor de displayAs               | Descrição
|:------------------------------|:-----------------------
| **account**                   | A cadeia de caracteres de declaração codificada bruta do SharePoint para a pessoa ou grupo (por exemplo. i:0#.f|membership|jane@contoso.com).
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
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
