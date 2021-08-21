---
title: 'governanceResource: register'
description: Registre um objeto governanceResource no PIM.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 05ab764e1cb4876889cc4627d1f94048990f61ff
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453860"
---
# <a name="governanceresource-register"></a>governanceResource: register

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registre [um objeto governanceResource](../resources/governanceresource.md) no Privileged Identity Management.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).

>**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.

### <a name="azure-resources"></a>Recursos do Azure

| Tipo de permissão | Permissões |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureResources |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

### <a name="azure-ad"></a>Microsoft Azure Active Directory

| Tipo de permissão | Permissões |
|:--------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureAD |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

### <a name="groups"></a>Grupos

|Tipo de permissão | Permissões |
|:-------------- |:----------- |
| Delegada (conta corporativa ou de estudante) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método **só dá** suporte aos `$select` `$expand` [parâmetros de consulta e OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
|:---- |:----------- |
| Autorização | Portador {token} |
| Content-type | application/json |

## <a name="request-body"></a>Corpo da solicitação

| Propriedades | Tipo | Descrição |
|:---------- |:---- |:----------- |
| externalId | Cadeia de caracteres | O identificador externo do recurso a ser registrado no PIM. Se registrar uma assinatura, o identificador será o identificador de assinatura pré-anexado por `/subscriptions/` . Por exemplo, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará uma `200 OK` resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como chamar essa API.
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a>Solicitação
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a>Resposta
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


