---
title: Tipo de recurso userFlowLanguagePage
description: As páginas de idioma de fluxo de usuário são usadas para determinar as cadeias de caracteres que os usuários serão mostrados durante a jornada do usuário que você configurou usando fluxos de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7a52d1dce81bc24809d788e8d28ef869b84c4704
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629515"
---
# <a name="userflowlanguagepage-resource-type"></a>Tipo de recurso userFlowLanguagePage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As páginas de idioma de fluxo de usuário são usadas para determinar as cadeias de caracteres que os usuários serão mostrados durante a jornada do usuário que você configurou usando fluxos de usuário. Essas páginas de idioma incluem as traduções de idioma padrão fornecidas pela Microsoft ou páginas personalizadas que podem ser criadas para personalizar as traduções de idioma.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userFlowLanguagePage](../api/userflowlanguagepage-get.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Recupere os valores de um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) padrão ou personalizado.|
|[Atualizar userFlowLanguagePage](../api/userflowlanguagepage-put.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Atualize os valores em um [objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) personalizado.|
|[Excluir userFlowLanguagePage](../api/userflowlanguagepage-delete.md)|Nenhum|Exclui os valores de um [objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) personalizado.|

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
