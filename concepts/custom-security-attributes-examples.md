---
title: Atribuir, atualizar ou remover atributos de segurança personalizados usando a API do Microsoft Graph (Visualização)
description: Saiba como atribuir, atualizar ou remover atributos de segurança personalizados para usuários e aplicativos (entidades de serviço) usando a API do Microsoft Graph.
author: rolyon
ms.localizationpriority: medium
ms.topic: how-to
ms.prod: directory-management
ms.openlocfilehash: 74603d7d39203134151928243de98624fc7a0dad
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077660"
---
# <a name="assign-update-or-remove-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>Atribuir, atualizar ou remover atributos de segurança personalizados usando a API do Microsoft Graph (Visualização)

> [!IMPORTANT]
> O recurso de atributos de segurança personalizados está atualmente em Visualização. Consulte os [Termos complementares](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) de Uso para visualizações Microsoft Azure para termos legais que se aplicam aos recursos do Azure que estão em beta, visualização ou que ainda não foram lançados em disponibilidade geral.

[Atributos de](/azure/active-directory/fundamentals/custom-security-attributes-overview) segurança personalizados no Azure Active Directory (Azure AD) são atributos específicos dos negócios (pares de valores-chave) que você pode definir e atribuir a objetos do Azure AD.

Este artigo fornece exemplos de como atribuir, atualizar ou remover diferentes tipos de atributos de segurança personalizados para usuários e aplicativos (entidades de serviço). Atributos de segurança personalizados podem ser atribuídos ou atualizados somente por meio de uma operação em um usuário `PATCH` [update](/graph/api/user-update?view=graph-rest-beta&preserve-view=true) ou [a solicitação Update servicePrincipal.](/graph/api/serviceprincipal-update?view=graph-rest-beta&preserve-view=true)

## <a name="permissions"></a>Permissões

Para gerenciar atributos de segurança personalizados, a entidade de chamada deve ser atribuída à seguinte função do Azure AD. Por padrão, o Administrador Global e outras funções de administrador não têm permissões para ler, definir ou atribuir atributos de segurança personalizados.

- [Administrador de Atribuição de Atributo](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

Além disso, a entidade de chamada deve ter a seguinte permissão.

- [CustomSecAttributeAssignment.ReadWrite.All](permissions-reference.md#custom-security-attributes-permissions)

## <a name="assign-custom-security-attributes"></a>Atribuir atributos de segurança personalizados

### <a name="example-1-assign-a-custom-security-attribute-with-a-string-value-to-a-user"></a>Exemplo 1: Atribuir um atributo de segurança personalizado com um valor de cadeia de caracteres a um usuário

O exemplo a seguir mostra como atribuir um atributo de segurança personalizado com um valor de cadeia de caracteres a um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `ProjectDate`
- Tipo de dados de atributo: Cadeia de caracteres
- Valor do atributo: `"2022-10-01"`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-assign-a-custom-security-attribute-with-a-string-value-to-a-service-principal"></a>Exemplo 2: Atribuir um atributo de segurança personalizado com um valor de cadeia de caracteres a uma entidade de serviço

O exemplo a seguir mostra como atribuir um atributo de segurança personalizado com um valor de cadeia de caracteres a uma entidade de serviço.

- Conjunto de atributos: `Engineering`
- Atributo: `ProjectDate`
- Tipo de dados de atributo: Cadeia de caracteres
- Valor do atributo: `"2022-10-01"`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "assign_serviceprincipal_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-3-assign-a-custom-security-attribute-with-a-multi-string-value-to-a-user"></a>Exemplo 3: Atribuir um atributo de segurança personalizado com um valor de várias cadeias de caracteres a um usuário

O exemplo a seguir mostra como atribuir um atributo de segurança personalizado com um valor de várias cadeias de caracteres a um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `Project`
- Tipo de dados de atributo: coleção de cadeias de caracteres
- Valor do atributo: `["Baker","Cascade"]`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_multistring"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Project@odata.type":"#Collection(String)",
            "Project":["Baker","Cascade"]
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-4-assign-a-custom-security-attribute-with-an-integer-value-to-a-user"></a>Exemplo 4: Atribuir um atributo de segurança personalizado com um valor inteiro a um usuário

O exemplo a seguir mostra como atribuir um atributo de segurança personalizado com um valor inteiro a um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `NumVendors`
- Tipo de dados de atributo: Integer
- Valor do atributo: `4`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_integer"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":4
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-5-assign-a-custom-security-attribute-with-a-multi-integer-value-to-a-user"></a>Exemplo 5: Atribuir um atributo de segurança personalizado com um valor multi-inteiro a um usuário

O exemplo a seguir mostra como atribuir um atributo de segurança personalizado com um valor multi-inteiro a um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `CostCenter`
- Tipo de dados de atributo: coleção de inteiros
- Valor do atributo: `[1001,1003]`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_multiinteger"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "CostCenter@odata.type":"#Collection(Int32)",
            "CostCenter":[1001,1003]
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-6-assign-a-custom-security-attribute-with-a-boolean-value-to-a-user"></a>Exemplo 6: Atribuir um atributo de segurança personalizado com um valor Boolean a um usuário

O exemplo a seguir mostra como atribuir um atributo de segurança personalizado com um valor Boolean a um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `Certification`
- Tipo de dados de atributo: Boolean
- Valor do atributo: `true`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_boolean"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Certification":true
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="update-custom-security-attribute-assignments"></a>Atualizar atribuições de atributo de segurança personalizadas

### <a name="example-1-update-a-custom-security-attribute-assignment-with-an-integer-value-for-a-user"></a>Exemplo 1: Atualizar uma atribuição de atributo de segurança personalizada com um valor inteiro para um usuário

O exemplo a seguir mostra como atualizar uma atribuição de atributo de segurança personalizada com um valor inteiro para um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `NumVendors`
- Tipo de dados de atributo: Integer
- Valor do atributo: `8`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "update_user_customsecurityattribute_integer"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":8
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-update-a-custom-security-attribute-assignment-with-a-boolean-value-for-a-user"></a>Exemplo 2: Atualizar uma atribuição de atributo de segurança personalizada com um valor Boolean para um usuário

O exemplo a seguir mostra como atualizar uma atribuição de atributo de segurança personalizada com um valor Boolean para um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `Certification`
- Tipo de dados de atributo: Boolean
- Valor do atributo: `false`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "update_user_customsecurityattribute_boolean"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Certification":false
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remove-custom-security-attribute-assignments"></a>Remover atribuições de atributo de segurança personalizadas

### <a name="example-1-remove-a-single-valued-custom-security-attribute-assignment-from-a-user"></a>Exemplo 1: Remover uma atribuição de atributo de segurança personalizada de valor único de um usuário

O exemplo a seguir mostra como remover uma atribuição de atributo de segurança personalizada que oferece suporte a um único valor de um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `ProjectDate`
- Valor do atributo: `null`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "remove_user_customsecurityattribute_singlevalue"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":null
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-multi-valued-custom-security-attribute-assignment-from-a-user"></a>Exemplo 2: Remover uma atribuição de atributo de segurança personalizada de vários valores de um usuário

O exemplo a seguir mostra como remover uma atribuição de atributo de segurança personalizada que oferece suporte a vários valores de um usuário.

- Conjunto de atributos: `Engineering`
- Atributo: `Project`
- Valor do atributo: `[]`

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "remove_user_customsecurityattribute_multivalue"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Project":[]
        }
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="next-steps"></a>Próximas etapas

- [Visão geral dos atributos de segurança personalizados usando a API Graph Microsoft](/graph/api/resources/custom-security-attributes-overview)
- [O que são atributos de segurança personalizados no Azure AD?](/azure/active-directory/fundamentals/custom-security-attributes-overview)
- [Atualizar usuário](/graph/api/user-update?view=graph-rest-beta&preserve-view=true)
- [Atualizar servicePrincipal](/graph/api/serviceprincipal-update?view=graph-rest-beta&preserve-view=true)
