---
title: Listar grupos
description: Liste todos os grupos disponíveis em uma organização, excluindo grupos dinâmicos de distribuição.
ms.localizationpriority: high
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d6ff0bba6e5d8f58d66c2a62270b6a75c17b9bab
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399226"
---
# <a name="list-groups"></a>Listar grupos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Liste todos os grupos disponíveis em uma organização, excluindo grupos dinâmicos de distribuição. Para recuperar grupos dinâmicos de distribuição, use o [Centro de administração do Exchange](/exchange/recipients/dynamic-distribution-groups/dynamic-distribution-groups).

Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada grupo. Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/group.md#properties). Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData. A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                                                                         |
| Aplicativo                            | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /groups
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método suporta aos parâmetros de consulta `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, e `$top` [OData](/graph/query-parameters) para ajudar a personalizar a resposta. Os tamanhos de página padrão e máximo são 100 e 999 objetos de grupo, respectivamente. Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

Para listar apenas grupos do Microsoft 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

O `$search` parâmetro de consulta suporta a tokenização apenas nos campos **displayName** e **description** e requer o cabeçalho **ConsistencyLevel**. Qualquer campo além de **displayName** e **description** é padrão para o comportamento`$filter``startswith`.

Para obter mais informações sobre as opções de consulta OData, veja [Parâmetros de consulta OData](/graph/query-parameters). Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome             | Descrição                                                                                                                                                                                                                                                                     |
| :--------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Autorização    | {token} de portador. Obrigatório.                                                                                                                                                                                                                                                       |
| ConsistencyLevel | eventualmente. Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries). |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta. A resposta inclui somente as propriedades padrão de cada grupo.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-a-list-of-groups"></a>Exemplo 1: Obter uma lista de grupos

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groups-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-groups-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-groups-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/get-groups-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
   "value":[
      {
         "id":"45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
         "deletedDateTime":null,
         "classification":null,
         "createdDateTime":"2018-12-22T02:21:05Z",
         "description":"Self help community for golf",
         "displayName":"Golf Assist",
         "expirationDateTime":null,
         "groupTypes":[
            "Unified"
         ],
         "isAssignableToRole":null,
         "mail":"golfassist@contoso.com",
         "mailEnabled":true,
         "mailNickname":"golfassist",
         "membershipRule":null,
         "membershipRuleProcessingState":null,
         "onPremisesLastSyncDateTime":null,
         "onPremisesSecurityIdentifier":null,
         "onPremisesSyncEnabled":null,
         "preferredDataLocation":"CAN",
         "preferredLanguage":null,
         "proxyAddresses":[
            "smtp:golfassist@contoso.onmicrosoft.com",
            "SMTP:golfassist@contoso.com"
         ],
         "renewedDateTime":"2018-12-22T02:21:05Z",
         "resourceBehaviorOptions":[
         ],
         "resourceProvisioningOptions":[
         ],
         "securityEnabled":false,
         "theme":null,
         "visibility":"Public",
         "onPremisesProvisioningErrors":[
         ]
      },
      {
         "id":"d7797254-3084-44d0-99c9-a3b5ab149538",
         "deletedDateTime":null,
         "classification":null,
         "createdDateTime":"2018-11-19T20:29:40Z",
         "description":"Talk about golf",
         "displayName":"Golf Discussion",
         "expirationDateTime":null,
         "groupTypes":[
         ],
         "isAssignableToRole":null,
         "mail":"golftalk@contoso.com",
         "mailEnabled":true,
         "mailNickname":"golftalk",
         "membershipRule":null,
         "membershipRuleProcessingState":null,
         "onPremisesLastSyncDateTime":null,
         "onPremisesSecurityIdentifier":null,
         "onPremisesSyncEnabled":null,
         "preferredDataLocation":"CAN",
         "preferredLanguage":null,
         "proxyAddresses":[
            "smtp:golftalk@contoso.onmicrosoft.com",
            "SMTP:golftalk@contoso.com"
         ],
         "renewedDateTime":"2018-11-19T20:29:40Z",
         "resourceBehaviorOptions":[
         ],
         "resourceProvisioningOptions":[
         ],
         "securityEnabled":false,
         "theme":null,
         "visibility":null,
         "onPremisesProvisioningErrors":[
         ]
      }
   ]
}
```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a>Exemplo 2: Obter uma lista filtrada de grupos, incluindo a contagem de objetos retornados

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

> **Observação:** os parâmetros de consulta `$count` e `$search` não estão disponíveis atualmente nos locatários do Azure Active Directory B2C.

<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a>Resposta

Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
   "@odata.count":2,
   "value":[
      {
         "id":"11111111-2222-3333-4444-555555555555",
         "displayName":"Contoso Group 1"
      },
      {
         "id":"22222222-3333-4444-5555-666666666666",
         "displayName":"Contoso Group 2"
      }
   ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a>Exemplo 3: Obter apenas uma contagem de grupos

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

> **Observação:** os parâmetros de consulta `$count` e `$search` não estão disponíveis atualmente nos locatários do Azure Active Directory B2C.

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a>Exemplo 4: Utilize $filter e $top para obter um grupo com um nome de exibição que comece com 'a', incluindo uma contagem de objetos retornados

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de caracteres de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

> **Observação:** os parâmetros de consulta `$count` e `$search` não estão disponíveis atualmente nos locatários do Azure Active Directory B2C.

<!-- {
  "blockType": "request",
  "name": "get_groups_startswith"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
   "@odata.count":1,
   "value":[
      {
         "displayName":"a",
         "mailNickname":"a241"
      }
   ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a>Exemplo 5: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$search` está na solicitação. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

> **Observação:** os parâmetros de consulta `$count` e `$search` não estão disponíveis atualmente nos locatários do Azure Active Directory B2C.

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
   "@odata.count":1396,
   "value":[
      {
         "displayName":"SFA Videos",
         "mail":"SFAVideos@service.contoso.com",
         "mailNickname":"SFAVideos"
      }
   ]
}
```

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a>Exemplo 6: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo' ou uma descrição que contenha as letras 'prod', incluindo uma contagem de objetos retornados

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$search` está na solicitação. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

> **Observação:** os parâmetros de consulta `$count` e `$search` não estão disponíveis atualmente nos locatários do Azure Active Directory B2C.

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
   "@odata.count":1396,
   "value":[
      {
         "displayName":"SFA Videos",
         "mail":"SFAVideos@service.contoso.com",
         "mailNickname":"SFAVideos"
      },
      {
         "description":"Video Production",
         "displayName":"Video Production",
         "mail":"videoprod@service.contoso.com",
         "mailNickname":"VideoProduction"
      }
   ]
}
```

### <a name="example-7-list-dynamic-groups"></a>Exemplo 7: listar grupos dinâmicos

#### <a name="request"></a>Solicitação

A seguir se encontra um exemplo da solicitação filtrada por **membershipRuleProcessingState** para recuperar grupos dinâmicos. Você também pode filtrar pelas propriedades **groupTypes** (ou seja, `$filter=groupTypes/any(s:s eq 'DynamicMembership')`). Essa solicitação requer o cabeçalho **ConsistencyLevel** definido como `eventual` e a `$count=true` cadeia de caracteres de consulta pois a solicitação usa o `not` operador do `$filter` parâmetro de consulta. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

> **Observação:** os parâmetros de consulta `$count` e `$search` não estão disponíveis atualmente nos locatários do Azure Active Directory B2C.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_enabled_dynamic_groups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'&$count=true&$select=id,membershipRule,membershipRuleProcessingState
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-enabled-dynamic-groups-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-enabled-dynamic-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-enabled-dynamic-groups-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-enabled-dynamic-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-enabled-dynamic-groups-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-enabled-dynamic-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-enabled-dynamic-groups-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-enabled-dynamic-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-enabled-dynamic-groups-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-enabled-dynamic-groups-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-enabled-dynamic-groups-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/get-enabled-dynamic-groups-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,membershipRule,membershipRuleProcessingState)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/e9f4a701-e7b5-4401-a0ca-5bd5f3cdcf4b/Microsoft.DirectoryServices.Group",
            "id": "e9f4a701-e7b5-4401-a0ca-5bd5f3cdcf4b",
            "membershipRule": "(user.userType -contains \"Guest\" and user.accountEnabled -eq true) or (user.city -eq \"Nairobi\")",
            "membershipRuleProcessingState": "On"
        }
    ]
}
```

### <a name="example-8-list-any-groups-with-any-licenses"></a>Exemplo 8: listar todos os grupos com licenças

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_groups_with_licenses"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$select=id,assignedLicenses&$filter=assignedLicenses/any()
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-with-licenses-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-with-licenses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-with-licenses-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-with-licenses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-with-licenses-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-with-licenses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-with-licenses-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-with-licenses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groups-with-licenses-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-groups-with-licenses-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-groups-with-licenses-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/get-groups-with-licenses-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,assignedLicenses)",
    "value": [
        {
            "id": "5caf712c-8483-4b3d-8384-d8da988c0ca4",
            "assignedLicenses": [
                {
                    "disabledPlans": [],
                    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900"
                }
            ]
        },
        {
            "id": "aae8ec2a-5a08-4013-ae70-fafbb5c20de1",
            "assignedLicenses": [
                {
                    "disabledPlans": [
                        "7547a3fe-08ee-4ccb-b430-5077c5041653"
                    ],
                    "skuId": "18181a46-0d4e-45cd-891e-60aabd171b4e"
                }
            ]
        },
        {
            "id": "e55bdaa0-e104-479a-979e-b0457fff6380",
            "assignedLicenses": [
                {
                    "disabledPlans": [
                        "7547a3fe-08ee-4ccb-b430-5077c5041653"
                    ],
                    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900"
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
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
