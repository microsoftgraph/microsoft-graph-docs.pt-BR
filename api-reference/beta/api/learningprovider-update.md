---
title: Atualizar learningProvider
description: Atualize as propriedades de um objeto learningProvider.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: ac9ced68d3e3bad6ac794a6641bd98997ceb7633
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883267"
---
# <a name="update-learningprovider"></a>Atualizar learningProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto learningProvider](../resources/learningprovider.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|LearningProvider.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /employeeExperience/learningProviders/{learningProviderId}
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
|displayName|Cadeia de caracteres|O nome de exibição que aparece Aprendizagem do Viva. Obrigatório.|
|isEnabled|Booliano|O estado do provedor. Opcional.|
|loginWebUrl|Cadeia de caracteres|URL de autenticação para acessar os cursos do provedor. Opcional.|
|longLogoWebUrlForDarkTheme|Cadeia de caracteres|A URL do logotipo longo para o modo escuro, que precisa ser uma imagem publicamente acessível. Essa imagem seria salva no Armazenamento de Blobs do Aprendizagem do Viva para renderização no Aprendizagem do Viva aplicativo. Obrigatório.|
|longLogoWebUrlForLightTheme|Cadeia de caracteres|A URL do logotipo longo para o modo claro, que precisa ser uma imagem publicamente acessível. Essa imagem seria salva no Armazenamento de Blobs do Aprendizagem do Viva para renderização no Aprendizagem do Viva aplicativo. Obrigatório.|
|squareLogoWebUrlForDarkTheme|Cadeia de caracteres|A URL do logotipo quadrado para o modo escuro, que precisa ser uma imagem acessível publicamente. Essa imagem seria salva no Armazenamento de Blobs do Aprendizagem do Viva para renderização no Aprendizagem do Viva aplicativo. Obrigatório.|
|squareLogoWebUrlForLightTheme|String|A URL do logotipo quadrado para o modo claro, que precisa ser uma imagem publicamente acessível. Essa imagem seria salva no Armazenamento de Blobs do Aprendizagem do Viva para renderização no Aprendizagem do Viva aplicativo. Obrigatório.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `204 No Content` código de resposta no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "update_learningprovider"
}
-->
``` http
PATCH /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70
Content-Type: application/json

{
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": false,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

