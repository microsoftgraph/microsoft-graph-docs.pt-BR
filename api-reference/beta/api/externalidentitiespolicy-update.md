---
title: Atualizar externalIdentitiesPolicy
description: Atualize as configurações do objeto externalIdentitiesPolicy em todo o locatário que controla se os usuários externos podem deixar um locatário Azure AD por meio de controles de autoatendimento.
author: KuiGithui
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 918bc089306c51d28a4afb61fc4a4038bb8eb049
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768338"
---
# <a name="update-externalidentitiespolicy"></a>Atualizar externalIdentitiesPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as configurações do objeto [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) em todo o locatário que controla se os usuários externos podem deixar um locatário Azure AD por meio de controles de autoatendimento.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.ExternalIdentities|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Policy.ReadWrite.ExternalIdentities|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/externalIdentitiesPolicy
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
|allowDeletedIdentitiesDataRemoval|Booliano|Notifica Azure AD se deve limpar as informações do usuário sobre a identidade externa, do locatário convidado, quando o usuário é excluído em seu locatário inicial. Obrigatório.|
|allowExternalIdentitiesToLeave|Boolean|Notifica Azure AD se deve limpar as informações do usuário sobre a identidade externa, do locatário convidado, quando o usuário é excluído em seu locatário inicial. Obrigatório.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_externalidentitiespolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/externalIdentitiesPolicy

{
  "allowExternalIdentitiesToLeave":false
}
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

