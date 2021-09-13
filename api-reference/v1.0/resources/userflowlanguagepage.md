---
title: Tipo de recurso userFlowLanguagePage
description: Determina as cadeias de caracteres mostradas aos usuários durante um fluxo de usuários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3c8367b29b857d7b1bce9dc5815ede5b74f5c025
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136310"
---
# <a name="userflowlanguagepage-resource-type"></a>Tipo de recurso userFlowLanguagePage

Namespace: microsoft.graph

Determina as páginas de idioma de fluxo do usuário que são mostradas aos usuários durante um fluxo de usuários. Essas páginas de idioma incluem as traduções de idioma padrão fornecidas pela Microsoft ou páginas personalizadas que podem ser criadas para personalizar as traduções de idioma.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userFlowLanguagePage](../api/userflowlanguagepage-get.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Recupere os valores de um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) padrão ou personalizado.|
|[Atualizar userFlowLanguagePage](../api/userflowlanguagepage-put.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Atualize os valores em um [objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) personalizado.|
|[Excluir userFlowLanguagePage](../api/userflowlanguagepage-delete.md)|Nenhum(a)|Exclui os valores de um [objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) personalizado.|

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
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
