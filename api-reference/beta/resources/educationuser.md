---
title: Tipo de recurso educationUser
description: Um usuário no sistema. Essa é uma variante específica de educação do usuário com a mesma `id` que o Microsoft Graph retornará do ponto de extremidade `/users` não específico da educação.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 22cdd5acc53de06458dd6ce986d635fc5ade2900
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292991"
---
# <a name="educationuser-resource-type"></a>Tipo de recurso educationUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um usuário no sistema. Essa é uma variante específica [] de educação do recurso de usuário padrão, com o mesmo que o Microsoft Graph retornará do ponto de extremidade não `id` específico para a `/users` educação.

Este objeto fornece um subconjunto direcionado de propriedades do objeto [de] usuário principal e adiciona um conjunto de propriedades específicas de `primaryRole` educação, como `student` , e `teacher` .

## <a name="methods"></a>Métodos

| Método                                               | Tipo de retorno                                  | Descrição                                                                   |
| :--------------------------------------------------- | :------------------------------------------- | :---------------------------------------------------------------------------- |
| [Obter educationUser](../api/educationuser-get.md)     | [educationUser]                              | Leia as propriedades e relações de um objeto **educationUser**.             |
| [Listar classes](../api/educationuser-list-classes.md) | Coleção [educationClass]                  | Obtenha a coleção de objetos **educationClass** da qual o usuário é membro.    |
| [Listar escolas](../api/educationuser-list-schools.md) | Coleção [educationSchool]                 | Obtenha a coleção de objetos **educationSchool** da qual o usuário é um membro. |
| [Obter usuário](../api/educationuser-get-user.md)         | [user]                                       | Obtenha o **user** do diretório simples que corresponde a esse **educationUser**. |
| [Atualizar](../api/educationuser-update.md)             | [educationUser]                              | Atualize um objeto **educationUser**.                                           |
| [Delete](../api/educationuser-delete.md)             | Nenhum                                         | Exclua um objeto **educationUser**.                                           |
| [Delta](../api/educationuser-delta.md)               | Coleção [educationUser](educationuser.md) | Obter alterações incrementais **para educationUsers**.                               |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                         | Descrição                                                                                                                                                                                   |
| :------------------- | :--------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                       | O identificador exclusivo do usuário. Herdado de [directoryObject]. Chave. Não anulável. Somente leitura.                                                                                           |
| accountEnabled       | Booliano                      | **True** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece \$ suporte ao filtro.                                                                |
| assignedLicenses     | Coleção [assignedLicense] | As licenças que são atribuídas ao usuário. Não anulável.                                                                                                                                     |
| assignedPlans        | Coleção [assignedPlan]    | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.                                                                                                                             |
| businessPhones       | Coleção de cadeias de caracteres            | Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                             |
| createdBy            | [identitySet]                | Entidade que criou o usuário.                                                                                                                                                                  |
| department           | String                       | O nome do departamento no qual o usuário trabalha. Oferece \$ suporte ao filtro.                                                                                                                       |
| displayName          | String                       | O nome exibido para o usuário no catálogo de endereços. Oferece suporte a $filter e $orderby.                                                                                                           |
| externalSource       | String                       | O tipo de fonte externa a partir da qual esse recurso foi gerado (determinado automaticamente a partir de `externalSourceDetail` ). Os valores possíveis são: `sis`, `lms` ou `manual`.                          |
| externalSourceDetail | String                       | O nome da fonte externa de onde esses recursos foram gerados.                                                                                                                            |
| givenName            | String                       | O nome fornecido (nome) do usuário. Oferece \$ suporte ao filtro.                                                                                                                                   |
| email                 | String                       | O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece \$ suporte ao filtro.                                                                                     |
| mailNickname         | String                       | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece \$ suporte ao filtro.                                                                                       |
| mailingAddress       | [physicalAddress]            | Endereço de email do usuário. Observação: `type` e não há suporte para `postOfficeBox` `educationUser` recursos.                                                                                       |
| middleName           | String                       | O nome do meio do usuário.                                                                                                                                                                      |
| mobilePhone          | String                       | O número de celular principal do usuário.                                                                                                                                           |
| onPremisesInfo       | [educationOnPremisesInfo]    | Informações adicionais usadas para associar o usuário do AAD ao seu equivalente do Active Directory.                                                                                                 |
| passwordPolicies     | String                       | Especifica as políticas de senha do usuário. Consulte o recurso [padrão] do usuário para obter detalhes adicionais.                                                                                                |
| passwordProfile      | [passwordProfile]            | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. Consulte o recurso [padrão] do usuário para obter detalhes adicionais. |
| preferredLanguage    | String                       | O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo, "en-US".                                                                                                      |
| primaryRole          | cadeia de caracteres                       | Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student`, `teacher`, `faculty`. Oferece \$ suporte ao filtro.                                  |
| provisionedPlans     | coleção [provisionedPlan] | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.                                                                                                                         |
| relatedContacts      | [coleção relatedContact]  | Registros relacionados ao usuário. As possíveis `parent` relações são , , , , , `relative` `aide` `doctor` `guardian` `child` `other` , `unknownFutureValue`                                    |
| residenceAddress     | [physicalAddress]            | Endereço em que o usuário reside. Observação: `type` e não há suporte para `postOfficeBox` `educationUser` recursos.                                                                                   |
| student              | [educationStudent]           | Se a função principal for aluno, esse bloco conterá dados específicos do aluno.                                                                                                                |
| surname              | String                       | O sobrenome do usuário (nome de família ou sobrenome). Oferece \$ suporte ao filtro.                                                                                                                             |
| teacher              | [educationTeacher]           | Se a função principal for o professor, esse bloco conterá dados específicos do professor.                                                                                                                |
| usageLocation        | String                       | Um código de país de duas letras ([ISO 3166 Alpha-2]). Obrigatório para os usuários que receberão licenças. Não anulável. Oferece \$ suporte ao filtro.                                                            |
| userPrincipalName    | String                       | O nome UPN do usuário. Oferece suporte a $filter e $orderby. Consulte o recurso [padrão] do usuário para obter detalhes adicionais.                                                               |
| userType             | String                       | Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Membro” e “Convidado”. Oferece \$ suporte ao filtro.                                                                    |

> [!IMPORTANT]
> Ao usar escopos de permissão delegados, o Graph retornará apenas um conjunto limitado de propriedades: `id` , , , , , , , `primaryRole` , `accountEnabled` `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` . `teacher/externalId` Se seu aplicativo exigir propriedades adicionais, você deverá usar escopos de permissão de aplicativo.

## <a name="relationships"></a>Relações

| Relação  | Tipo                         | Descrição                                  |
| :------------ | :--------------------------- | :------------------------------------------- |
| assignments   | [educationAssignment]        | Lista de atribuições para o usuário. Anulável.  |
| classes       | Coleção [educationClass]  | Aulas às quais o usuário pertence. Anulável. |
| schools       | Coleção [educationSchool] | Escolas às quais o usuário pertence. Anulável. |
| taughtClasses | Coleção [educationClass]  | Aulas para as quais o usuário é professor.     |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "accountEnabled": true,
  "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
  "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
  "businessPhones": ["String"],
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "department": "String",
  "displayName": "String",
  "externalSource": "string",
  "givenName": "String",
  "id": "String (identifier)",
  "mail": "String",
  "mailNickname": "String",
  "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
  "middleName": "String",
  "mobilePhone": "String",
  "officeLocation": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  },
  "passwordPolicies": "String",
  "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
  "preferredLanguage": "String",
  "primaryRole": "string",
  "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
  "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
  "student": { "@odata.type": "microsoft.graph.educationStudent" },
  "surname": "String",
  "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]

}-->

[educationuser]: educationuser.md
[educationclass]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: educationassignment.md
[educationteacher]: educationteacher.md
[educationstudent]: educationstudent.md
[relatedcontact]: relatedcontact.md
[physicaladdress]: physicaladdress.md
[provisionedplan]: provisionedplan.md
[passwordprofile]: passwordprofile.md
[identityset]: identityset.md
[assignedplan]: assignedplan.md
[assignedlicense]: assignedlicense.md
[user]: user.md
[directoryobject]: directoryobject.md
[educationonpremisesinfo]: educationonpremisesinfo.md
[iso 3166 alpha-2]: https://www.iso.org/obp/ui/#search
[rfc 822]: https://tools.ietf.org/html/rfc822


