---
author: JeremyKelley
description: O recurso FolderView fornece ou define recomendações sobre a experiência do usuário de uma pasta.
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9657e22104f621cf59bab48c40e6aaab911dd08c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058442"
---
# <a name="folderview-resource-type"></a>Tipo de recurso FolderView

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **FolderView** fornece ou define recomendações sobre a experiência do usuário de uma pasta.

Está disponível a partir da propriedade [folder][folder-facet] dos recursos [driveItem][item-resource].

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade         | Tipo   | Descrição
|:----------------------|:-------|:--------------------------------------------
| **sortBy**            | string | O método pelo qual a pasta deve ser classificada.
| **sortOrder**         | string | Se for verdadeiro, indica que os itens devem ser classificados em ordem decrescente. Caso contrário, os itens devem ser classificados em ordem crescente.
| **viewType**          | string | O tipo de modo de exibição que deve ser usado para representar a pasta.

Você pode usar a propriedade _sortBy_ para controlar a ordem de classificação dos itens em aplicativos que respeitam a faceta **viewType**.

### <a name="sortby-values"></a>Valores sortBy

Os seguintes valores são definidos para a propriedade **sortBy**.

| Valor                    | Descrição
| ------------------------ | --------------------------------------------------
| `default`                | A ordem de classificação padrão do aplicativo.
| `name`                   | Os itens devem ser organizados pela propriedade **name** dos itens.
| `type`                   | Os itens devem ser organizados pelo tipo de item.
| `size`                   | Os itens devem ser organizados pela propriedade **size** dos itens.
| `takenOrCreatedDateTime` | Os itens devem ser organizados pela propriedade **takenDateTime** da faceta **photo**. Se não estiver disponível, a propriedade **createdDateTime** deverá ser usada.
| `lastModifiedDateTime`   | Os itens devem ser organizados pela propriedade **lastModifiedDateTime** dos itens.
| `sequence`               | Os itens seguem uma sequência personalizada especificada pelo usuário.


### <a name="sortorder-values"></a>Valores sortOrder

Os seguintes valores são definidos para a propriedade **sortOrder**.

| Valor        | Descrição
| ------------ | --------------------------------------------------------------
| `ascending`  | Os itens devem ser organizados em ordem crescente.
| `descending` | Os itens devem ser organizados em ordem decrescente.


### <a name="viewtype-values"></a>Valores viewType

Os seguintes valores são definidos para a propriedade **viewType**.

| Valor        | Descrição
| ------------ | --------------------------------------------------------------
| `default`    | O tipo de exibição padrão para o aplicativo.
| `icons`      | Um modo de exibição que usa ícones para representar driveItems.
| `details`    | Um modo de exibição com várias colunas que fornecem detalhes adicionais sobre cada item.
| `thumbnails` | Um modo de exibição que usa miniaturas maiores de driveItems para representar os itens.


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


