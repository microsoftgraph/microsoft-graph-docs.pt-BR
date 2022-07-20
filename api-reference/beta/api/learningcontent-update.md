---
title: Atualizar learningContent
description: Atualize as propriedades de um objeto learningContent.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: 80e9caa91d973e90e0f7b8d9f4ccb07708dbdb4f
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883263"
---
# <a name="update-learningcontent"></a>Atualizar learningContent
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize o recurso [learningContent](../resources/learningcontent.md) especificado. 

Usado por um [provedor de aprendizado](../resources/learningprovider.md) para ingerir ou atualizar os metadados para seu conteúdo Aprendizagem do Viva. Se o conteúdo de aprendizado especificado ainda não existir para o provedor especificado, essa operação criará os metadados para o novo conteúdo. Caso contrário, essa operação substituirá os metadados do conteúdo existente.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|LearningContent.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|LearningContent.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /employeeExperience/learningProviders/{registrationId}/learningContents(externalId='{externalId}') 
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|additionalTags|String collection|Palavras-chave, tópicos e outras marcas associadas ao conteúdo de aprendizado. Opcional.|
|contentWebUrl|String|A URL da Web de conteúdo para o conteúdo de aprendizado. Obrigatório.|
|Contribuinte|String|O autor, criador ou colaborador do conteúdo de aprendizado. Opcional.|
|createdDateTime|DateTimeOffset|A data em que o conteúdo de aprendizado foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional.|
|descrição|Cadeia de caracteres|A descrição ou resumo do conteúdo de aprendizado. Opcional.|
|duração|Duração|A duração do conteúdo de aprendizado em segundos. Opcional.|
|externalId|Cadeia de caracteres|ID de conteúdo externo exclusiva para o conteúdo de aprendizado. Obrigatório.|
|format|Cadeia de caracteres|O formato do conteúdo de aprendizado. Por exemplo, `Course`, `Video`, `Book`, `Book Summary`, `Audiobook Summary`. Opcional.|
|isActive|Booliano|Indica se o conteúdo está ativo ou não. O conteúdo inativo não será exibido na interface do usuário. O valor padrão é `true`. Opcional.|
|isPremium|Booliano|Indica se o conteúdo de aprendizado exige que o usuário entre na plataforma do provedor de aprendizagem ou não. O valor padrão é `false`. Opcional.|
|Issearchable|Booliano|Indica se o conteúdo de aprendizado é pesquisável ou não. O valor padrão é `true`. Opcional.|
|languageTag|String|O idioma do conteúdo de aprendizado, por exemplo, `en-us` ou `fr-fr`. Obrigatório.|
|lastModifiedDateTime|DateTimeOffset|A data em que o conteúdo de aprendizado foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional.|
|numberOfPages|Int32|O número de páginas do conteúdo de aprendizado, por exemplo, 9. Opcional.|
|skillTags|Coleção String|As marcas de habilidades associadas ao conteúdo de aprendizado. Opcional.|
|Sourcename|String|O nome de origem do conteúdo de aprendizado, como `LinkedIn Learning` ou `Coursera`. Opcional.|
|thumbnailWebUrl|Cadeia de caracteres|A URL da imagem em miniatura do conteúdo de aprendizagem. Opcional.|
|title|Cadeia de caracteres|O título do conteúdo de aprendizado. Obrigatório.|



## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `202 Accepted` de resposta e um objeto [learningContent](../resources/learningcontent.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "update_learningcontent"
}
-->
``` http
PATCH /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70/learningContents(externalId='LP4471') 
Content-Type: application/json

{
    "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
    "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
    "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
    "sourceName": "MsLearn",
    "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
    "languageTag": "en-us",
    "numberOfPages": 9,
    "duration": "PT20M",
    "format": "Book",
    "createdDateTime": "2018-01-01T00:00:00",
    "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
    "contributor": "Scott Simpson",
    "additionalTags": [
        "Create private or public teams",
        "Add members to teams"
    ],
    "skillTags": [
        "Create teams",
        "Teams channels",
        "Teams members"
    ],
    "isActive": true,
    "isPremium": false,
    "isSearchable": true
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.learningContent"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#learningProviders('13727311-e7bb-470d-8b20-6a23d9030d70')/learningContents/$entity",
    "externalId": "LP4471",
    "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
    "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
    "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
    "sourceName": "MsLearn",
    "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
    "languageTag": "en-us",
    "numberOfPages": 9,
    "duration": "PT20M",
    "format": "Book",
    "createdDateTime": "2018-01-01T00:00:00",
    "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
    "contributor": "Scott Simpson",
    "additionalTags": [
        "Create private or public teams",
        "Add members to teams"
    ],
    "skillTags": [
        "Create teams",
        "Teams channels",
        "Teams members"
    ],
    "isActive": true,
    "isPremium": false,
    "isSearchable": true
}
```

