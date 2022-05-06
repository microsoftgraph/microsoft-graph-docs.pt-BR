---
title: 'administrativeUnit: delta'
description: Obtenha unidades administrativas recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos.
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2e47c63784bbab4fa0d549ae638cbe7a8dd479f7
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246661"
---
# <a name="administrativeunit-delta"></a>administrativeUnit: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha **administrativeUnits** recém-criados, atualizados ou excluídos sem precisar executar uma leitura completa de toda a coleção de recursos. Para obter detalhes, consulte [Usando a consulta delta](/graph/delta-query-overview).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|administrativeunit | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para começar a controlar as alterações, você faz uma solicitação que inclui a função delta no **recurso administrativeUnit** .

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

Controlar alterações incorre em uma rodada de uma ou mais **chamadas de função delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `@odata.nextLink` ou `@odata.deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta uma vez antecipadamente. Em solicitações subsequentes, copie e aplique `@odata.nextLink` a URL `@odata.deltaLink` da resposta anterior. Essa URL já inclui os parâmetros codificados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de](/graph/delta-query-overview) estado retornado na `@odata.deltaLink` URL da chamada de função **delta anterior** para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações. Salve e aplique toda a URL `@odata.deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.|
| $skiptoken | string | Um [token de](/graph/delta-query-overview) estado retornado na `@odata.nextLink` URL da chamada de função **delta anterior** , indicando que há mais alterações a serem controladas na mesma coleção de recursos. |

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método suporta os seguintes parâmetros de consulta OData para ajudar a personalizar a resposta:

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade **id** sempre será retornada. 

- Há suporte limitado para `$filter`:
  * A única expressão com suporte `$filter` é para controlar alterações para recursos específicos, por sua ID:  `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}`. O número de IDs que você pode especificar é limitado pelo comprimento máximo da URL.


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;token&gt; de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` o código de resposta e um objeto [de coleção administrativeUnit](../resources/administrativeunit.md) no corpo da resposta. A resposta também inclui uma URL `@odata.nextLink` ou uma URL `@odata.deltaLink`. 

- Se uma URL `@odata.nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. A **administrativeUnit continua** fazendo solicitações usando `@odata.nextLink` a URL até que uma `@odata.deltaLink` URL seja incluída na resposta.

- Se uma URL `@odata.deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Persista e use `@odata.deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.

Para obter detalhes e um exemplo, consulte [Using delta query and](/graph/delta-query-overview) [Get incremental changes for users](/graph/delta-query-users).

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "administrativeunit_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/administrativeunit-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/administrativeunit-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/administrativeunit-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/administrativeunit-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/administrativeunit-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/administrativeunit-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#administrativeunits",
  "@odata.nextLink":"https://graph.microsoft.com/beta/administrativeunits/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Management Fast Track",
      "visibility": null,
      "extension_fe2174665583431c953114ff7268b7b3_Education_ObjectType": "School",
      "extension_fe2174665583431c953114ff7268b7b3_Education_StateId": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Address": "2 Microsoft Way",
      "extension_fe2174665583431c953114ff7268b7b3_Education_City": "Redmond",
      "extension_fe2174665583431c953114ff7268b7b3_Education_State": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Country": "US",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Zip": "98052",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Phone": "555-123-4567",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource": "SIS",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource_SchoolId": "10002",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalSyncSourceId": "14008",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalName": "Amy Roebuck",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalEmail": "aroebuck@principal.edu",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolZone": "1",
      "id": "8a07f5a8-edc9-4847-bbf2-dde106594bf4",
      "members@delta": [
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "b66ecf79-a093-4d51-86e0-efcc4531f37a"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "5bde3e51-d13b-4db1-9948-fe4b109d11a7"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "801f2093-de7e-4883-a786-8a5f30874ff4"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "7e4ec76c-8276-43ef-ba10-9aaa197cb212"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "f5289423-7233-4d60-831a-fe107a8551cc"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "48d31887-5fad-4d73-a9f5-3c356e68a038"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "c03e6eaa-b6ab-46d7-905b-73ec7ea1f755"
        }
      ]
  }
  ]
}
```

<!-- uuid: 69848a18-6b48-44fd-a398-4521803a0a00
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeunit: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


