---
title: tipo de recurso userFlowLanguagePage
description: Páginas de idioma de fluxo do usuário são usadas determine as cadeias de caracteres que os usuários serão mostrados durante a jornada do usuário que você configurou usando fluxos de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d6a6bd597fb274d8fdb8150be0a2c5e085949156
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706214"
---
# <a name="userflowlanguagepage-resource-type"></a>tipo de recurso userFlowLanguagePage

Namespace: microsoft.graph

Páginas de idioma de fluxo do usuário são usadas determine as cadeias de caracteres que os usuários serão mostrados durante a jornada do usuário que você configurou usando fluxos de usuário. Essas páginas de idioma incluem as traduções de idioma padrão fornecidas pela Microsoft ou páginas personalizadas que podem ser criadas para personalizar as traduções de idiomas.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userFlowLanguagePage](../api/userflowlanguagepage-get.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Recupere os valores de um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) padrão ou personalizado.|
|[Atualizar userFlowLanguagePage](../api/userflowlanguagepage-put.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Atualizar os valores em um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) personalizado.|
|[Excluir userFlowLanguagePage](../api/userflowlanguagepage-delete.md)|Nenhum|Exclui os valores de um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) personalizado.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da página userFlowLanguage.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
