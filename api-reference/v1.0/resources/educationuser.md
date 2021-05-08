---
title: Tipo de recurso educationUser
description: Um usuário no sistema. Essa é uma variante específica de educação do usuário com a mesma `id` que o Microsoft Graph retornará do ponto de extremidade `/users` não específico da educação.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 012e181d9f95ff8b3c145c8a7a0e8a70b14cf625
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231826"
---
# <a name="educationuser-resource-type"></a>Tipo de recurso educationUser

Namespace: microsoft.graph

Um usuário no sistema. Essa é uma variante específica de educação do usuário com a mesma `id` que o Microsoft Graph retornará do ponto de extremidade `/users` não específico da educação. Esse objeto fornece um subconjunto direcionado de propriedades do objeto principal [user](../resources/user.md) e adiciona um conjunto de propriedades específico de educação, como dados de `primaryRole`, aluno e professor.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

| Método                                                           | Tipo de retorno                                                 | Descrição                                                                                        |
| :--------------------------------------------------------------- | :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------- |
| [Listar educationUsers](../api/educationuser-list.md)              | Coleção [educationUser](../resources/educationuser.md)   | Obter uma lista dos [objetos educationUser](../resources/educationuser.md) e suas propriedades.     |
| [Criar educationUser](../api/educationuser-post.md)           | [educationUser](../resources/educationuser.md)              | Crie um novo [objeto educationUser.](../resources/educationuser.md)                                |
| [Obter educationUser](../api/educationuser-get.md)                 | [educationUser](../resources/educationuser.md)              | Leia as propriedades e as relações de um [objeto educationUser.](../resources/educationuser.md) |
| [Atualizar educationUser](../api/educationuser-update.md)           | [educationUser](../resources/educationuser.md)              | Atualize as propriedades de um [objeto educationUser.](../resources/educationuser.md)                 |
| [Excluir educationUser](../api/educationuser-delete.md)           | Nenhum                                                        | Exclua um objeto [educationUser](../resources/educationuser.md).                                  |
| [delta](../api/educationuser-delta.md)                           | Coleção [educationUser](../resources/educationuser.md)   | Obter alterações incrementais na coleção de recursos.                                                |
| [Listar taughtClasses](../api/educationuser-list-taughtclasses.md) | Coleção [educationClass](../resources/educationclass.md) | Obter os recursos educationClass da propriedade de navegação de classes ensinadas.                       |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                                               | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| :------------------- | :----------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Booliano                                                            | `True` se a conta estiver habilitada; caso contrário, `false`. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                                                    |
| assignedLicenses     | Coleção [assignedLicense](../resources/assignedlicense.md)      | As licenças que são atribuídas ao usuário. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| assignedPlans        | Coleção [assignedPlan](../resources/assignedplan.md)            | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| businessPhones       | Coleção de cadeias de caracteres                                                  | Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                                                                                                                                                                                                                                                                                                                                                                |
| createdBy            | [identitySet](../resources/identityset.md)                         | Entidade que criou o usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| department           | String                                                             | O nome do departamento no qual o usuário trabalha. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| displayName          | String                                                             | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte para `$filter` e `$orderby`.                                                                                                                                                                                                                                                           |
| externalSource       | educationExternalSource                                            | De onde esse usuário foi criado. Os valores possíveis são: `sis` e `manual`.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| externalSourceDetail | String                                                             | O nome da fonte externa de onde esses recursos foram gerados.                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| givenName            | String                                                             | O nome fornecido (nome) do usuário. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| id                   | String                                                             | Identificador de objeto. Herdado da [entidade](../resources/entity.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| email                 | String                                                             | O endereço SMTP do usuário; por exemplo, jeff@contoso.onmicrosoft.com. Somente Leitura. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | Endereço de email do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| mailNickname         | String                                                             | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                           |
| middleName           | String                                                             | O nome do meio do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mobilePhone          | String                                                             | O número de celular principal do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | Informações adicionais usadas para associar o usuário do Azure AD ao seu equivalente do Active Directory.                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| passwordPolicies     | String                                                             | Especifica as políticas de senha do usuário. Este valor é uma enumeração com um valor possível sendo `DisableStrongPassword`, que permite que senhas mais fracas do que a política padrão sejam especificadas. `DisablePasswordExpiration` também pode ser especificado. Os dois podem ser especificados juntos; por exemplo: `DisablePasswordExpiration, DisableStrongPassword` .                                                                                                                                                                      |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.                                                                                                                                                                                                                             |
| preferredLanguage    | String                                                             | O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo, "en-US".                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| primaryRole          | educationUserRole                                                  | Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student`, `teacher`, `none`, `unknownFutureValue`.                                                                                                                                                                                                                                                                                                                                                                     |
| provisionedPlans     | coleção [provisionedPlan](../resources/provisionedplan.md)      | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | Endereço em que o usuário reside.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| showInAddressList    | Booliano                                                            | true se a lista de endereços global do Outlook deve conter o usuário, caso contrário false. Se não estiver configurado, isso será tratado como true. Para os usuários convidados por meio do Gerenciador de convites, essa propriedade será definida como false.                                                                                                                                                                                                                                                                                                               |
| student              | [educationStudent](../resources/educationstudent.md)               | Se a função principal for aluno, esse bloco conterá dados específicos do aluno.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| surname              | String                                                             | O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | Se a função primária for professor, esse bloco conterá dados específicos do professor.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| usageLocation        | String                                                             | Um código de país de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços em países ou regiões. Os exemplos incluem: "US", "JP" e "GB". Não anulável. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                |
| userPrincipalName    | String                                                             | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, onde o domínio deve estar presente na coleta de domínios verificados pelo locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). Oferece suporte para `$filter` e `$orderby`. |
| userType             | String                                                             | Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Membro” e “Convidado”. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                        |

> [!IMPORTANT]
> Ao usar escopos de permissão delegados, Graph retornará apenas um conjunto limitado de propriedades: `id` , , , , , , , , , `primaryRole` , `accountEnabled` , `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` `teacher/externalId` . Se seu aplicativo exigir propriedades adicionais, você deve usar escopos de permissão application.

## <a name="relationships"></a>Relações

| Relação  | Tipo                                                          | Descrição                                    |
| :------------ | :------------------------------------------------------------ | :--------------------------------------------- |
| classes       | Coleção [educationClass](../resources/educationclass.md)   | Aulas às quais o usuário pertence. Anulável.   |
| schools       | Coleção [educationSchool](../resources/educationschool.md) | Escolas às quais o usuário pertence. Anulável.   |
| taughtClasses | Coleção [educationClass](../resources/educationclass.md)   | Classes para as quais o usuário é professor.       |
| usuário          | [user](../resources/user.md)                                  | O usuário de diretório correspondente a esse usuário. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "String (identifier)",
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
  "businessPhones": ["String"],
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: microsoft.graph.educationUser/assignments:
      Referenced type microsoft.graph.educationAssignment is not defined in the doc set! Potential suggestion: UNKNOWN"
  ],
  "tocPath": ""
}-->

[educationuser]: educationuser.md
[educationclass]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: /graph/api/resources/educationassignment?view=graph-rest-beta
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

