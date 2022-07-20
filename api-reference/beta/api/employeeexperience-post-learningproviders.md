---
title: Criar learningProvider
description: Crie um novo objeto learningProvider.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: 40655e18f4fe22b3417f9ef2166538810ae36de4
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883249"
---
# <a name="create-learningprovider"></a>Criar learningProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto learningProvider](../resources/learningprovider.md) e registre-o com Aprendizagem do Viva usando o nome de exibição e logotipos especificados para temas diferentes.

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
POST /employeeExperience/learningProviders
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto learningProvider](../resources/learningprovider.md) .

Você pode especificar as propriedades a seguir ao criar um **learningProvider**.

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

Se bem-sucedido, este método retorna um código `201 Created` de resposta e um [objeto learningProvider](../resources/learningprovider.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_learningprovider_from_"
}
-->
``` http
POST /employeeExperience/learningProviders 
Content-Type: application/json

{
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": true,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.learningProvider"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#learningProviders/$entity",
    "id": "ba9790ef-21d5-4c17-808c-acda55230253",
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": true,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```

