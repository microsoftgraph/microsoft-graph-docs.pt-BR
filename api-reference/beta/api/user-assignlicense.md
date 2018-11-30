---
title: assignLicense
description: Adicionar ou remover licenças do usuário habilitar ou desabilitar o uso de ofertas de nuvem da Microsoft. Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com 100 licenças e essa solicitação atribui uma dessas licenças a usuários específicos. Você também pode ativar e desativar os planos de específicos associados a uma assinatura. Para saber mais sobre licenças e assinaturas, consulte este artigo do Technet.
ms.openlocfilehash: ecfe1f97e2e951998e0a62eea68412279eae524f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041179"
---
# <a name="assignlicense"></a>assignLicense

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Adicionar ou remover licenças do usuário habilitar ou desabilitar o uso de ofertas de nuvem da Microsoft. Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com 100 licenças e essa solicitação atribui uma dessas licenças a usuários específicos. Você também pode ativar e desativar os planos de específicos associados a uma assinatura. Para saber mais sobre licenças e assinaturas, consulte este [artigo do Technet](https://technet.microsoft.com/en-us/library/mt765146.aspx).

Para obter as assinaturas disponíveis no diretório, execute um [obter subscribedSkus solicitação](subscribedsku-list.md). 

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadWrite.All, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|addLicenses|Coleção [assignedLicense](../resources/assignedlicense.md)|Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especificam as licenças para adicionar. Você pode desabilitar servicePlans associados com uma licença, definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md) .|
|removeLicenses|Guid|Uma coleção de skuIds que identificam as licenças para remover.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` código de resposta e um objeto de [usuário](../resources/user.md) de atualizada no corpo da resposta.

## <a name="example"></a>Exemplo
Adicione licenças ao usuário.
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```

## <a name="example"></a>Exemplo
Remova licenças de usuário.

#####<a name="request"></a>Solicitação
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a>Resposta
Nos dois exemplos, a resposta é o objeto de usuário atualizada. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
