---
title: Atualizar trustFrameworkPolicy
description: 'Esta operação atualiza um objeto trustFrameworkPolicy existente ou, se houver algum, ele cria um. '
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9807802d426fc5069a83014e52f0ed2210e05102
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027346"
---
# <a name="update-or-create-trustframeworkpolicy"></a>Atualizar ou criar trustFrameworkPolicy

Namespace: microsoft.graph

>**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Atualize um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) existente ou crie um se ele não existir.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|Policy.ReadWrite.TrustFramework|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|Policy.ReadWrite.TrustFramework|

A conta corporativa ou de estudante deve ser um administrador global do locatário.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|Application/XML. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação XML do objeto [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) . 

>**Observação:** o tipo de conteúdo deve ser `application/xml` .

## <a name="response"></a>Resposta

A resposta será uma das seguintes:
- Se existir um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) , uma solicitação bem-sucedida retornará um `200 OK` código de resposta.
- Se não existir um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) , uma solicitação com êxito retornará um `201 Created` código de resposta.
- Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="example"></a>Exemplo

O exemplo a seguir atualiza um **trustFrameworkPolicy**.

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a>Resposta

<!-- {
  "blockType": "ignored",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_Test" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    .....
    ....
    <!---PolicyContent-->
    ....
    ....
</TrustFrameworkPolicy>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update trustframeworkpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


