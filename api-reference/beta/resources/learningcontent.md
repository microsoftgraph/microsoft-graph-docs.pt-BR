---
title: Tipo de recurso learningContent
description: Representa uma entidade que contém detalhes sobre o conteúdo de aprendizado.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: resourcePageType
ms.openlocfilehash: 865070a402c68327a1fef41b6c793e5672f878c3
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883243"
---
# <a name="learningcontent-resource-type"></a>Tipo de recurso learningContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os metadados do conteúdo para aprendizado de funcionários.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar learningContents](../api/learningprovider-list-learningcontents.md)|[Coleção learningContent](../resources/learningcontent.md)|Obtenha uma lista dos recursos [learningContent](../resources/learningcontent.md) e suas propriedades. Essa lista representa os metadados do conteúdo do provedor especificado em Aprendizagem do Viva.|
|[Obter learningContent](../api/learningcontent-get.md)|[learningContent](../resources/learningcontent.md)|Obtenha o recurso learningContent especificado, que representa os metadados do conteúdo ingerido do provedor especificado.|
|[Atualizar learningContent](../api/learningcontent-update.md)|[learningContent](../resources/learningcontent.md)|Atualize o recurso [learningContent](../resources/learningcontent.md) especificado. Usado por um [provedor de aprendizado](learningprovider.md) para ingerir ou atualizar os metadados para seu conteúdo Aprendizagem do Viva.|
|[Excluir learningContent](../api/learningprovider-delete-learningcontents.md)|Nenhum|Exclua o recurso learningContent especificado que representa os metadados do conteúdo ingerido do provedor especificado.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|additionalTags|Coleção de cadeias de caracteres|Palavras-chave, tópicos e outras marcas associadas ao conteúdo de aprendizado. Opcional.|
|contentWebUrl|Cadeia de caracteres|A URL da Web de conteúdo para o conteúdo de aprendizado. Obrigatório.|
|Contribuinte|Cadeia de caracteres|O autor, criador ou colaborador do conteúdo de aprendizado. Opcional.|
|createdDateTime|DateTimeOffset|A data em que o conteúdo de aprendizado foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional.|
|descrição|Cadeia de caracteres|A descrição ou resumo do conteúdo de aprendizado. Opcional.|
|duração|Duração|A duração do conteúdo de aprendizado em segundos. Opcional.|
|externalId|Cadeia de caracteres|ID de conteúdo externo exclusiva para o conteúdo de aprendizado. Obrigatório.|
|format|String|O formato do conteúdo de aprendizado. Por exemplo, `Course`, `Video`, `Book`, `Book Summary`, `Audiobook Summary`. Opcional.|
|isActive|Booliano|Indica se o conteúdo está ativo ou não. O conteúdo inativo não será exibido na interface do usuário. O valor padrão é `true`. Opcional.|
|isPremium|Booliano|Indica se o conteúdo de aprendizado exige que o usuário entre na plataforma do provedor de aprendizagem ou não. O valor padrão é `false`. Opcional.|
|Issearchable|Booliano|Indica se o conteúdo de aprendizado é pesquisável ou não. O valor padrão é `true`. Opcional.|
|languageTag|String|O idioma do conteúdo de aprendizado, por exemplo, `en-us` ou `fr-fr`. Obrigatório.|
|lastModifiedDateTime|DateTimeOffset|A data em que o conteúdo de aprendizado foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional.|
|numberOfPages|Int32|O número de páginas do conteúdo de aprendizado, por exemplo, 9. Opcional.|
|skillTags|Coleção String|As marcas de habilidades associadas ao conteúdo de aprendizado. Opcional.|
|Sourcename|Cadeia de caracteres|O nome de origem do conteúdo de aprendizado, como `LinkedIn Learning` ou `Coursera`. Opcional.|
|thumbnailWebUrl|Cadeia de caracteres|A URL da imagem em miniatura do conteúdo de aprendizagem. Opcional.|
|title|Cadeia de caracteres|O título do conteúdo de aprendizado. Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.learningContent",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.learningContent",
    "additionalTags": [
        "String"
    ],
    "contentWebUrl": "String",
    "contributor": "String",
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "duration": "String (duration)",
    "externalId": "String",
    "format": "String",
    "isActive": "Boolean",
    "isPremium": "Boolean",
    "isSearchable": "Boolean",
    "languageTag": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "numberOfPages": "Integer",
    "skillTags": [
        "String"
    ],
    "sourceName": "String",
    "thumbnailWebUrl": "String",
    "title": "String"
}
```

