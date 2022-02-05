---
title: Atualizar accessPackageCatalog
description: Atualize as propriedades de um objeto accessPackageCatalog.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
---
# <a name="update-accesspackagecatalog"></a>Atualizar accessPackageCatalog

Namespace: microsoft.graph


Atualize um objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) existente para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}
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
|displayName|String|O nome do catálogo de pacotes de acesso.|
|description|String|A descrição do catálogo de pacotes de acesso.|
|catalogType|accessPackageCatalogType|Se o catálogo é criado por um usuário ou gerenciamento de direitos. Os valores possíveis são: `userManaged`, `serviceDefault`, `serviceManaged`, `unknownFutureValue`.|
|state|accessPackageCatalogState|Tem o valor `published` se os pacotes de acesso estão disponíveis para gerenciamento. Os valores possíveis são: `unpublished`, `published`, `unknownFutureValue`.|
|isExternallyVisible|Booliano|Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `204 No Content`.



## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
```http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}
Content-Type: application/json

{
  "displayName":"Catalog One"
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
}
-->
```http
HTTP/1.1 204 No Content
Content-Type: application/json

```

