---
title: Registrar governanceResource
description: Registre um objeto governanceResource não gerenciado no PIM.
localization_priority: Normal
ms.openlocfilehash: ce439d53eb9f017340f561ca509e8da43dbafbfc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837748"
---
# <a name="register-governanceresource"></a>Registrar governanceResource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Registre um objeto não gerenciado [governanceResource](../resources/governanceresource.md) no gerenciamento de identidades privilegiado.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Essa API também requer que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.

|Tipo de permissão      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método **só** oferece suporte a `$select` e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

### <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | Portador {código}|
| Content-type  | application/json|

### <a name="request-body"></a>Corpo da solicitação

|Parâmetros      |Tipo                 |Obrigatório |Descrição|
|:-------------|:----------------------|:--------|:----------|
|externalId    |Cadeia de caracteres                 |✓        |ExternalId do recurso a ser registrado no PIM.|

### <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` resposta.

### <a name="example"></a>Exemplo
Este exemplo mostra como registrar uma assinatura do Azure Wingtip Toys - produção.
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
<!-- {
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
