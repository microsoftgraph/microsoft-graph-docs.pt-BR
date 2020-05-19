---
title: 'aplicativo: removeKey'
description: Remover uma credencial de chave de um aplicativo
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2395d2372b70d6ed3150c8186803d3d3226acaba
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289144"
---
# <a name="application-removekey"></a>aplicativo: removeKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Remover uma credencial de chave de um [aplicativo](../resources/application.md). Este método junto com o [addKey](application-addkey.md) pode ser usado por um aplicativo para automatizar a interrupção de suas chaves de expiração.

> [!NOTE]
> [Criar o servicePrincipalName](../api/serviceprincipal-post-serviceprincipals.md) e [Atualizar](../api/serviceprincipal-update.md) as operações do servicePrincipalName podem continuar a ser usado para adicionar e atualizar as principais credenciais de qualquer aplicativo com o aplicativo ou o contexto de um usuário.

Como parte da solicitação de validação para esse método, uma prova de posse de uma chave existente é verificada antes que a ação possa ser executada.

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Nenhum  |
|Delegado (conta pessoal da Microsoft) | Nenhum.    |
|Aplicativo | Nenhum |

> [!NOTE] 
> Um aplicativo não precisa de nenhuma permissão específica para rolar suas próprias chaves.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removeKey
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição                |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça as seguintes propriedades obrigatórias.

| Propriedade  | Tipo | Descrição|
|:----------|:-----|:-----------|
| keyId     | GUID | O identificador exclusivo da senha.|
| evidência | String | Um token JWT auto-assinado usado como prova de posse das chaves existentes. Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo. O token deve conter as seguintes declarações:<ul><li>`aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .</li><li>`iss`– O emissor precisa ser a __ID__ do aplicativo que está fazendo a chamada.</li><li>`nbf`-Não antes da hora.</li><li>`exp`– O tempo de expiração deve ser "NBF" + 10 minutos.</li></ul><br>Veja a seguir um [exemplo](/graph/application-rollkey-prooftoken) de código que pode ser usado para gerar esse token de prova de posse.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No content`.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "application_removekey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->