---
title: Atualizar educationUser
description: Atualize as propriedades de um objeto educationUser.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 002b61a29a245902e458a70c03aacc4982b9d2ad
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024594"
---
# <a name="update-educationuser"></a>Atualizar educationUser

Namespace: microsoft.graph

Atualize as propriedades de um [objeto educationUser.](../resources/educationuser.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Sem suporte.  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | EduRoster.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade             | Tipo                                                               | Descrição                                                                                                                                                                                                                                                                                                                                                 |
| :------------------- | :----------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Boolean                                                            | **True** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.                                                                                                                                                                                                                               |
| assignedLicenses     | Coleção [assignedLicense](../resources/assignedlicense.md)      | As licenças que são atribuídas ao usuário. Não anulável.                                                                                                                                                                                                                                                                                                   |
| assignedPlans        | Coleção [assignedPlan](../resources/assignedplan.md)            | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                           |
| businessPhones       | Coleção de cadeias de caracteres                                                  | Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                                                                                                                                                                                           |
| createdBy            | [identitySet](../resources/identityset.md)                         | Entidade que criou o usuário.                                                                                                                                                                                                                                                                                                                                |
| departamento           | String                                                             | O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                      |
| displayName          | String                                                             | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.                                                                                      |
| externalSource       | educationExternalSource                                            | De onde esse usuário foi criado. Os valores possíveis são: `sis` e `manual`.                                                                                                                                                                                                                                                                                     |
| externalSourceDetail | Cadeia de caracteres                                                             | O nome da fonte externa de onde esses recursos foram gerados.                                                                                                                                                                                                                                                                                          |
| givenName            | String                                                             | O nome fornecido (nome) do usuário. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                  |
| email                 | String                                                             | O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a $filter.                                                                                                                                                                                                                                                    |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | Endereço de email do usuário.                                                                                                                                                                                                                                                                                                                                       |
| mailNickname         | String                                                             | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.                                                                                                                                                                                                                                                      |
| middleName           | String                                                             | O nome do meio do usuário.                                                                                                                                                                                                                                                                                                                                    |
| mobilePhone          | String                                                             | O número de celular principal do usuário.                                                                                                                                                                                                                                                                                                         |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | Informações adicionais usadas para associar o AAD usuário ao seu equivalente do Active Directory.                                                                                                                                                                                                                                                               |
| passwordPolicies     | String                                                             | Especifica as políticas de senha do usuário. Este valor é uma enumeração com um possível valor sendo "DisableStrongPassword", que permite especificar as senhas mais fracas do que a política padrão. O "DisablePasswordExpiration" também pode ser especificado. Os dois podem ser especificados juntos, por exemplo: "DisablePasswordExpiration, DisableStrongPassword". |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.                                                        |
| preferredLanguage    | String                                                             | O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo, "en-US".                                                                                                                                                                                                                                                                    |
| primaryRole          | educationUserRole                                                  | Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student`, `teacher`, `none`, `unknownFutureValue`.                                                                                                                                                                                                |
| provisionedPlans     | coleção [provisionedPlan](../resources/provisionedplan.md)      | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                       |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | Endereço em que o usuário reside.                                                                                                                                                                                                                                                                                                                                   |
| student              | [educationStudent](../resources/educationstudent.md)               | Se a função principal for aluno, esse bloco conterá dados específicos do aluno.                                                                                                                                                                                                                                                                              |
| surname              | String                                                             | O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.                                                                                                                                                                                                                                                                                            |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | Se a função primária for professor, esse bloco conterá dados específicos do professor.                                                                                                                                                                                                                                                                              |
| usageLocation        | String                                                             | Um código de país de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços em países ou regiões. Os exemplos incluem: "US", "JP" e "GB". Não anulável. Oferece suporte a $filter.                                                                                           |
| userPrincipalName    | String                                                             | O nome UPN do usuário.                                                                                                                                                                                                                                                                                                                  |
| userType             | String                                                             | Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como "Member" e "Guest". Oferece suporte a $filter.                                                                                                                                                                                                                                   |

## <a name="response"></a>Resposta
Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-educationuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
