---
title: 'virtualEndpoint: getEffectivePermissions'
description: '**GetEffectivePermissions é uma função que Retrives as permissões efetivas do usuário atualmente autenticado, o que ajuda o UX a ocultar ou desabilitar o conteúdo ao qual o usuário atual não tem acesso.**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 78b58c5ea00e1b170d831a91f5dc3ff1569bd0d7
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378261"
---
# <a name="virtualendpoint-geteffectivepermissions"></a>virtualEndpoint: getEffectivePermissions

Namespace: microsoft.graph

Exibir as permissões efetivas do usuário autenticado no momento. GetEffectivePermissions é uma função que Retrives as permissões efetivas do usuário atualmente autenticado, o que ajuda o UX a ocultar ou desabilitar o conteúdo ao qual o usuário atual não tem acesso.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC. ReadWrite. All, CloudPC. Read. All|
|Delegado (conta pessoal da Microsoft) | Sem suporte.|
|Aplicativo| Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta. Se o usuário tiver permissões completas, a resposta será `["*"]` .

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    "Microsoft.CloudPC/CloudPCs/Read"
  ]
}
```
