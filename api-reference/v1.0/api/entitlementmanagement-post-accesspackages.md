---
title: Criar accessPackage
description: Crie um novo accessPackage.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e9c62d3444f65f0d17dadc26070ffe8afe18eb7d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242157"
---
# <a name="create-accesspackage"></a>Criar accessPackage

Namespace: microsoft.graph

Crie um novo [objeto accessPackage.](../resources/accesspackage.md)

O pacote de acesso será adicionado a um [accessPackageCatalog existente.](../resources/accesspackagecatalog.md)

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
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | \{token\} de portador. Obrigatório. |
| Content-type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto accessPackage.](../resources/accesspackage.md)

Você pode especificar as seguintes propriedades ao criar **um accessPackage**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do pacote de acesso.|
|description|Cadeia de caracteres|A descrição do pacote de acesso.|
|IsHidden|Booleano|Se o pacote de acesso está oculto do solicitante.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto accessPackage](../resources/accesspackage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_accesspackage"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages
Content-Type: application/json

{
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "catalog": {
    "id": "66584aae-98bb-48cc-9458-7bee5d2a6577"
  }
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "642181f0-bc17-4fc6-9ebb-ff53dbf18c2f",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "createdDateTime": "2021-11-10T01:10:09.5220119Z",
  "modifiedDateTime": "2021-11-10T01:10:09.5220119Z"
}
```

