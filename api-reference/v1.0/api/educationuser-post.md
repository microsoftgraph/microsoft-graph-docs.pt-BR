---
title: Criar educationUser
description: Crie um novo objeto educationUser.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b26e0530fd4beea6d2f604fa46f891e154fefa61
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232144"
---
# <a name="create-educationuser"></a>Criar educationUser

Namespace: microsoft.graph

Crie um novo [objeto educationUser.](../resources/educationuser.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Sem suporte.                              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/users
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto educationUser.](../resources/educationuser.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [educationUser](../resources/educationuser.md).

| Propriedade             | Tipo                                                               | Descrição                                                                                                                                                                                                                                                                                                                                                 |
| :------------------- | :----------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Booliano                                                            | **True** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.                                                                                                                                                                                                                               |
| assignedLicenses     | Coleção [assignedLicense](../resources/assignedlicense.md)      | As licenças que são atribuídas ao usuário. Não anulável.                                                                                                                                                                                                                                                                                                   |
| assignedPlans        | Coleção [assignedPlan](../resources/assignedplan.md)            | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                           |
| businessPhones       | Coleção de cadeias de caracteres                                                  | Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                                                                                                                                                                                           |
| createdBy            | [identitySet](../resources/identityset.md)                         | Entidade que criou o usuário.                                                                                                                                                                                                                                                                                                                                |
| department           | String                                                             | O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                      |
| displayName          | String                                                             | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.                                                                                      |
| externalSource       | educationExternalSource                                            | De onde esse usuário foi criado. Os valores possíveis são: `sis` e `manual`.                                                                                                                                                                                                                                                                                     |
| externalSourceDetail | String                                                             | O nome da fonte externa de onde esses recursos foram gerados.                                                                                                                                                                                                                                                                                          |
| givenName            | String                                                             | O nome fornecido (nome) do usuário. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                  |
| email                 | String                                                             | O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a $filter.                                                                                                                                                                                                                                                    |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | Endereço de email do usuário.                                                                                                                                                                                                                                                                                                                                       |
| mailNickname         | String                                                             | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.                                                                                                                                                                                                                                                      |
| middleName           | String                                                             | O nome do meio do usuário.                                                                                                                                                                                                                                                                                                                                    |
| mobilePhone          | String                                                             | O número de celular principal do usuário.                                                                                                                                                                                                                                                                                                         |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | Informações adicionais usadas para associar o usuário do AAD ao equivalente do Active Directory.                                                                                                                                                                                                                                                               |
| passwordPolicies     | String                                                             | Especifica as políticas de senha do usuário. Este valor é uma enumeração com um possível valor sendo "DisableStrongPassword", que permite especificar as senhas mais fracas do que a política padrão. O "DisablePasswordExpiration" também pode ser especificado. Os dois podem ser especificados juntos, por exemplo: "DisablePasswordExpiration, DisableStrongPassword". |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.                                                        |
| preferredLanguage    | String                                                             | O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo, "en-US".                                                                                                                                                                                                                                                                    |
| primaryRole          | educationUserRole                                                  | Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student`, `teacher`, `none`.                                                                                                                                                                                                                      |
| provisionedPlans     | coleção [provisionedPlan](../resources/provisionedplan.md)      | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                       |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | Endereço em que o usuário reside.                                                                                                                                                                                                                                                                                                                                   |
| student              | [educationStudent](../resources/educationstudent.md)               | Se a função principal for aluno, esse bloco conterá dados específicos do aluno.                                                                                                                                                                                                                                                                              |
| surname              | String                                                             | O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.                                                                                                                                                                                                                                                                                            |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | Se a função primária for professor, esse bloco conterá dados específicos do professor.                                                                                                                                                                                                                                                                              |
| usageLocation        | String                                                             | Um código de país de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços em países ou regiões. Os exemplos incluem: "US", "JP" e "GB". Não anulável. Oferece suporte a $filter.                                                                                           |
| userPrincipalName    | String                                                             | O nome UPN do usuário.                                                                                                                                                                                                                                                                                                                  |
| userType             | String                                                             | Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como "Member" e "Guest". Oferece suporte a $filter.                                                                                                                                                                                                                                   |

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/users
Content-Type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.educationUser",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```

### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```
