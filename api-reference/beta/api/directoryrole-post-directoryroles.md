---
title: Ativar directoryRole
description: Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente as funções de diretório administradores da empresa e usuários implícitos são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef4e7ed1661309ea40a3a573fe5b830f65da7c88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957651"
---
# <a name="activate-directoryrole"></a>Ativar directoryRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente as funções de diretório administradores da empresa e usuários implícitos são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement. ReadWrite. Directory |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).

A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.

|Parâmetro obrigatório | Tipo | Descrição|
|:---------|:---------|:---------|
|roleTemplateId | string | A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
