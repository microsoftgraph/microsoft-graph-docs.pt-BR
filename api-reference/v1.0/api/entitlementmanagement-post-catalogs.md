---
title: Criar accessPackageCatalog
description: Crie um novo accessPackageCatalog.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 043df8315a4f91953555fb36fbd2458ec363af82
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242198"
---
# <a name="create-accesspackagecatalog"></a>Criar accessPackageCatalog

Namespace: microsoft.graph


Crie um novo [objeto accessPackageCatalog.](../resources/accesspackagecatalog.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/catalogs
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | \{token\} de portador. Obrigatório. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto accessPackageCatalog.](../resources/accesspackagecatalog.md)

Você pode especificar as seguintes propriedades ao criar **um accessPackageCatalog**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do catálogo de pacotes de acesso.|
|description|Cadeia de caracteres|A descrição do catálogo de pacotes de acesso.|
|state|accessPackageCatalogState|Tem o valor `published` se os pacotes de acesso estão disponíveis para gerenciamento. Os valores possíveis são: `unpublished` e `published` .|
|isExternallyVisible|Booliano|Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs
Content-Type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "state": "published",
  "isExternallyVisible": true
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{

  "id": "b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "userManaged",
  "state": "published",
  "isExternallyVisible": true,
  "createdDateTime": "2021-11-10T01:08:30.9134953Z",
  "modifiedDateTime": "2021-11-10T01:08:30.9134953Z"
}
```

