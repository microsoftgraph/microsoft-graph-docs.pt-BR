---
title: Tipo de recurso educationUser
description: Um usuário no sistema. Essa é uma variante específica de educação do usuário com a mesma `id` que o Microsoft Graph retornará do ponto de extremidade `/users` não específico da educação.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b3e193a49d1668d43fb311c5e43a506daaa5688a
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685079"
---
# <a name="educationuser-resource-type"></a>Tipo de recurso educationUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um usuário no sistema. Essa é uma variante específica da educação do recurso de [] usuário padrão, `id` com o mesmo que o Microsoft Graph retornará `/users` do ponto de extremidade não específico da educação.

Esse objeto fornece [] um subconjunto `primaryRole`de propriedades de destino do objeto de usuário principal e adiciona um conjunto de propriedades específicas da educação, como , `student`e .`teacher`

## <a name="methods"></a>Métodos

| Método                                               | Tipo de retorno                                  | Descrição                                                                   |
| :--------------------------------------------------- | :------------------------------------------- | :---------------------------------------------------------------------------- |
| [Obter educationUser](../api/educationuser-get.md)     | [educationUser]                              | Leia as propriedades e relações de um objeto **educationUser**.             |
| [Listar classes](../api/educationuser-list-classes.md) | Coleção [educationClass]                  | Obtenha a coleção de objetos **educationClass** da qual o usuário é membro.    |
| [Listar escolas](../api/educationuser-list-schools.md) | Coleção [educationSchool]                 | Obtenha a coleção de objetos **educationSchool** da qual o usuário é um membro. |
| [Obter usuário](../api/educationuser-get-user.md)         | [user]                                       | Obtenha o **user** do diretório simples que corresponde a esse **educationUser**. |
| [Atualizar](../api/educationuser-update.md)             | [educationUser]                              | Atualize um objeto **educationUser**.                                           |
| [Delete](../api/educationuser-delete.md)             | Nenhuma                                         | Exclua um objeto **educationUser**.                                           |
| [Delta](../api/educationuser-delta.md)               | Coleção [educationUser](educationuser.md) | Obter alterações incrementais para **educationUsers**.                               |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                         | Descrição                                                                                                                                                                                   |
| :------------------- | :--------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                       | O identificador exclusivo do usuário. Herdado de [directoryObject]. Chave. Não anulável. Somente leitura.                                                                                           |
| accountEnabled       | Booliano                      | **True** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Dá suporte ao \$filtro.                                                                |
| assignedLicenses     | Coleção [assignedLicense] | As licenças que são atribuídas ao usuário. Não anulável.                                                                                                                                     |
| assignedPlans        | Coleção [assignedPlan]    | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.                                                                                                                             |
| businessPhones       | String collection            | Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                             |
| createdBy            | [identitySet]                | Entidade que criou o usuário.                                                                                                                                                                  |
| department           | String                       | O nome do departamento no qual o usuário trabalha. Dá suporte ao \$filtro.                                                                                                                       |
| displayName          | String                       | O nome exibido para o usuário no catálogo de endereços. Oferece suporte a $filter e $orderby.                                                                                                           |
| externalSource       | String                       | O tipo de fonte externa da qual esse recurso foi gerado (determinado automaticamente de `externalSourceDetail`). Os valores possíveis são: `sis`, `lms` ou `manual`.                          |
| externalSourceDetail | Cadeia de caracteres                       | O nome da fonte externa da qual esses recursos foram gerados.                                                                                                                            |
| givenName            | String                       | O nome fornecido (nome) do usuário. Dá suporte ao \$filtro.                                                                                                                                   |
| email                 | String                       | O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Dá suporte ao \$filtro.                                                                                     |
| mailNickname         | String                       | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Dá suporte ao \$filtro.                                                                                       |
| mailingAddress       | [physicalAddress]            | Endereço de email do usuário. Observação: `type` e `postOfficeBox` não há suporte para recursos `educationUser` .                                                                                       |
| middleName           | String                       | O nome do meio do usuário.                                                                                                                                                                      |
| mobilePhone          | String                       | O número de celular principal do usuário.                                                                                                                                           |
| onPremisesInfo       | [educationOnPremisesInfo]    | Informações adicionais usadas para associar AAD usuário ao seu equivalente do Active Directory.                                                                                                 |
| passwordPolicies     | String                       | Especifica as políticas de senha do usuário. Consulte o recurso [de usuário] padrão para obter detalhes adicionais.                                                                                                |
| passwordProfile      | [passwordProfile]            | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. Consulte o recurso [de usuário] padrão para obter detalhes adicionais. |
| preferredLanguage    | String                       | O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo, "en-US".                                                                                                      |
| primaryRole          | cadeia de caracteres                       | Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student`, `teacher`, `faculty`. Dá suporte ao \$filtro.                                  |
| provisionedPlans     | coleção [provisionedPlan] | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.                                                                                                                         |
| relatedContacts      | [coleção relatedContact]  | Registros relacionados relacionados ao usuário. As relações possíveis `parent`são , `relative`, `aide`, `doctor`, `guardian`, `child`, , `other``unknownFutureValue`                                    |
| residenceAddress     | [physicalAddress]            | Endereço em que o usuário reside. Observação: `type` e `postOfficeBox` não há suporte para recursos `educationUser` .                                                                                   |
| student              | [educationStudent]           | Se a função principal for aluno, esse bloco conterá dados específicos do aluno.                                                                                                                |
| surname              | String                       | O sobrenome do usuário (nome de família ou sobrenome). Dá suporte ao \$filtro.                                                                                                                             |
| teacher              | [educationTeacher]           | Se a função principal for professor, esse bloco conterá dados específicos do professor.                                                                                                                |
| usageLocation        | String                       | Um código de país de duas letras ([ISO 3166 Alpha-2]). Necessário para usuários que receberão licenças. Não anulável. Dá suporte ao \$filtro.                                                            |
| userPrincipalName    | String                       | O nome UPN do usuário. Oferece suporte a $filter e $orderby. Consulte o recurso [de usuário] padrão para obter detalhes adicionais.                                                               |
| userType             | String                       | Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Membro” e “Convidado”. Dá suporte ao \$filtro.                                                                    |

> [!IMPORTANT]
> Ao usar escopos de permissão delegados, Graph retornará apenas um conjunto limitado de propriedades: , , , , `displayName`, `givenName``surname`, , `userPrincipalName`, `userType`, `onPremisesInfo`, `student/externalId`. `teacher/externalId``accountEnabled``primaryRole``id` Se o aplicativo exigir propriedades adicionais, você deverá usar escopos de permissão do aplicativo.

## <a name="relationships"></a>Relações

| Relação  | Tipo                         | Descrição                                  |
| :------------ | :--------------------------- | :------------------------------------------- |
| assignments   | [educationAssignment]        | Lista de atribuições para o usuário. Anulável.  |
| classes       | Coleção [educationClass]  | Aulas às quais o usuário pertence. Anulável. |
| schools       | Coleção [educationSchool] | Escolas às quais o usuário pertence. Anulável. |
| taughtClasses | Coleção [educationClass]  | Classes para as quais o usuário é professor.     |
|Rubricas|[coleção educationRubric](educationrubric.md)|Quando definido, a rubrica de classificação anexada à atribuição.|

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
[Physicaladdress]: physicaladdress.md
[provisionedplan]: provisionedplan.md
[passwordprofile]: passwordprofile.md
[identityset]: identityset.md
[plano atribuído]: assignedplan.md
[assignedlicense]: assignedlicense.md
[user]: user.md
[directoryobject]: directoryobject.md
[educationonpremisesinfo]: educationonpremisesinfo.md
[iso 3166 alpha-2]: https://www.iso.org/obp/ui/#search
[rfc 822]: https://tools.ietf.org/html/rfc822


