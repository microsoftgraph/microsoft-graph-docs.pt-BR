---
title: Registrar Entidadegovernanceresource
description: Registre um objeto Entidadegovernanceresource não gerenciado no PIM.
localization_priority: Normal
ms.openlocfilehash: a6ad89f799ee171971f7301ed039cf1b6d9111ea
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329737"
---
# <a name="register-governanceresource"></a>Registrar Entidadegovernanceresource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registre um objeto [entidadegovernanceresource](../resources/governanceresource.md) não gerenciado no gerenciamento de identidade privilegiado.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.

|Tipo de permissão      | Permissões              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess. ReadWrite. AzureResources  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | PrivilegedAccess. ReadWrite. AzureResources |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método **só** oferece suporte `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

### <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Authorization  | Portador {código}|
| Content-type  | application/json|

### <a name="request-body"></a>Corpo da solicitação

|Parâmetros      |Tipo                 |Obrigatório |Descrição|
|:-------------|:----------------------|:--------|:----------|
|externalId    |Cadeia de caracteres                 |✓        |ExternalId do recurso a ser registrado no PIM.|

### <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` uma resposta.

### <a name="example"></a>Exemplo
Este exemplo mostra como registrar uma assinatura do Azure na Wingtip Toys-prod.
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>Solicitação
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
