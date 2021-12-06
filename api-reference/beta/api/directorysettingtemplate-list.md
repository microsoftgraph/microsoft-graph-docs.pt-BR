---
title: Listar directorySettingTemplates
description: Essa operação recupera a lista de objetos directorySettingTemplates disponíveis.
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bed83bd03998cf6366b2e3693ead62a036b48d77
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998919"
---
# <a name="list-directorysettingtemplates"></a>Listar directorySettingTemplates

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os modelos de configuração de diretório representam um conjunto de modelos de configurações de diretório, a partir dos quais as configurações de diretório podem ser criadas e usadas em um locatário.  Essa operação recupera a lista de objetos **directorySettingTemplates** disponíveis.

> **Observação**: a versão /beta dessa API só se aplica a grupos. A versão /v1.0 desta API foi renomeada para *List groupSettingTemplate*.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directorysettingtemplates-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directorySettingTemplates",
  "value": [
    {
      "id": "08d542b9-071f-4e16-94b0-74abb372e3d9",
      "deletedDateTime": null,
      "displayName": "Group.Unified.Guest",
      "description": "Settings for a specific Unified Group",
      "values": [
        {
          "name": "AllowToAddGuests",
          "type": "System.Boolean",
          "defaultValue": "true",
          "description": "Flag indicating if guests are allowed in a specific Unified Group."
        }
      ]
    },
    {
      "id": "80661d51-be2f-4d46-9713-98a2fcaec5bc",
      "deletedDateTime": null,
      "displayName": "Prohibited Names Settings",
      "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for managing tenant-wide prohibited names settings.",
      "values": [
        {
          "name": "CustomBlockedSubStringsList",
          "type": "System.String",
          "defaultValue": "",
          "description": "A comma delimited list of substring reserved words to block for application display names."
        },
        {
          "name": "CustomBlockedWholeWordsList",
          "type": "System.String",
          "defaultValue": "",
          "description": "A comma delimited list of reserved words to block for application display names."
        }
      ]
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


