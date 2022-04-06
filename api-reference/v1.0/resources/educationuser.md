---
title: Tipo de recurso educationUser
description: Representa um usuário no sistema. Esta é uma variante específica da educação do usuário com a mesma ID que a Microsoft Graph retornará do ponto de extremidade /usuários não específicos da educação.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d1e7ffe90690b35b25537a9ca23d9b8f05d9817c
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588537"
---
# <a name="educationuser-resource-type"></a>Tipo de recurso educationUser

Namespace: microsoft.graph

Um usuário no sistema. Esta é uma variante específica da educação do usuário com a mesma **id** que a Microsoft Graph retornará do ponto de extremidade não específico `/users` da educação. Este objeto fornece um subconjunto direcionado de propriedades do objeto de [usuário principal e](../resources/user.md) adiciona um conjunto de propriedades específicas da educação, como **dados primaryRole**, **student** **e teacher** .

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

| Método                                                           | Tipo de retorno                                                 | Descrição                                                                                        |
| :--------------------------------------------------------------- | :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------- |
| [Listar educationUsers](../api/educationuser-list.md)              | Coleção [educationUser](../resources/educationuser.md)   | Obter uma lista dos [objetos educationUser](../resources/educationuser.md) e suas propriedades.     |
| [Criar educationUser](../api/educationuser-post.md)             | [educationUser](../resources/educationuser.md)              | Crie um novo [objeto educationUser](../resources/educationuser.md) .                                |
| [Obter educationUser](../api/educationuser-get.md)                 | [educationUser](../resources/educationuser.md)              | Leia as propriedades e as relações de um [objeto educationUser](../resources/educationuser.md) . |
| [Atualizar educationUser](../api/educationuser-update.md)           | [educationUser](../resources/educationuser.md)              | Atualize as propriedades de um [objeto educationUser](../resources/educationuser.md) .                 |
| [Excluir educationUser](../api/educationuser-delete.md)           | Nenhum                                                        | Exclua um objeto [educationUser](../resources/educationuser.md).                                   |
| [delta](../api/educationuser-delta.md)                           | Coleção [educationUser](../resources/educationuser.md)   | Obter alterações incrementais na coleção de recursos.                                                |
| [Listar taughtClasses](../api/educationuser-list-taughtclasses.md) | Coleção [educationClass](../resources/educationclass.md) | Obter os **recursos educationClass** da **propriedade de navegação de classes ensinadas** .                       |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                                               | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| :------------------- | :----------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Booliano                                                            | `True` se a conta estiver habilitada; caso contrário, `false`. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                |
| assignedLicenses     | Coleção [assignedLicense](../resources/assignedlicense.md)      | As licenças que são atribuídas ao usuário. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| assignedPlans        | Coleção [assignedPlan](../resources/assignedplan.md)            | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| businessPhones       | String collection                                                  | Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                                                                                                                                                                                                                                                                                                                                                                        |
| createdBy            | [identitySet](../resources/identityset.md)                         | A entidade que criou o usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| department           | String                                                             | O nome do departamento no qual o usuário trabalha. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| displayName          | String                                                             | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte para `$filter` e `$orderby`.                                                                                                                                                                                                                                                               |
| externalSource       | educationExternalSource                                            | De onde esse usuário foi criado. Os valores possíveis são: `sis` e `manual`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| externalSourceDetail | Cadeia de caracteres                                                             | O nome da fonte externa de onde esse recurso foi gerado.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| givenName            | String                                                             | O nome fornecido (nome) do usuário. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| id                   | Cadeia de caracteres                                                             | Identificador de objeto. Herdado da [entidade](../resources/entity.md).                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| email                 | String                                                             | O endereço SMTP do usuário, por exemplo, `jeff@contoso.onmicrosoft.com`. Somente Leitura. Suporta o `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | O endereço de email do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| mailNickname         | String                                                             | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| middleName           | String                                                             | O nome do meio do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| mobilePhone          | String                                                             | O número de celular principal do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | Informações adicionais usadas para associar o usuário Azure Active Directory seu equivalente do Active Directory.                                                                                                                                                                                                                                                                                                                                                                                                                          |
| passwordPolicies     | String                                                             | Especifica as políticas de senha do usuário. Este valor é uma enumeração com um valor possível sendo `DisableStrongPassword`, que permite que senhas mais fracas do que a política padrão sejam especificadas. `DisablePasswordExpiration` também pode ser especificado. Os dois podem ser especificados juntos; por exemplo: `DisablePasswordExpiration, DisableStrongPassword`.                                                                                                                                                                              |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.                                                                                                                                                                                                                                     |
| preferredLanguage    | Cadeia de caracteres                                                             | O idioma preferencial para o usuário que deve seguir o código ISO 639-1, por exemplo, `en-US`.                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| primaryRole          | educationUserRole                                                  | Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student`, `teacher`, `none`, `unknownFutureValue`.                                                                                                                                                                                                                                                                                                                                                                             |
| provisionedPlans     | coleção [provisionedPlan](../resources/provisionedplan.md)      | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| relatedContacts      | [coleção relatedContact]                                        | Registros relacionados associados ao usuário. Somente leitura.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | O endereço onde o usuário mora.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| showInAddressList    | Booliano                                                            | `True`se a Outlook de endereços global deve conter esse usuário; caso contrário, `false`. Se não estiver configurado, isso será tratado como `true`. Para os usuários convidados por meio do Gerenciador de convites, essa propriedade será definida como `false`.                                                                                                                                                                                                                                                                                                               |
| student              | [educationStudent](../resources/educationstudent.md)               | Se a função principal for aluno, esse bloco conterá dados específicos do aluno.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| surname              | String                                                             | O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | Se a função primária for professor, esse bloco conterá dados específicos do professor.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| usageLocation        | String                                                             | Um código de país de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços em países ou regiões. Os exemplos incluem:`US`,`JP` e `GB`. Não anulável. Oferece suporte para `$filter`.                                                                                                                                                                                                                                                                      |
| userPrincipalName    | String                                                             | O nome UPN do usuário. O UPN é um nome de logon no estilo internet para o usuário com base no RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é `alias@domain`, onde o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados a partir da **propriedade verifiedDomains** da [organização](organization.md). Oferece suporte para `$filter` e `$orderby`. |
| userType             | String                                                             | Um valor de string que pode ser usado para classificar tipos de usuário em seu diretório, como `Member` e `Guest`. Suporta o `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                              |

> [!IMPORTANT]
> Ao usar escopos de permissão delegados, o Microsoft Graph retornará apenas um conjunto limitado de propriedades: **id**, **primaryRole**, **accountEnabled**, **displayName**, **givenName**, **surname**, **userPrincipalName**, **userType**, **onPremisesInfo**, **student/externalId**, **teacher/externalId**. Se seu aplicativo exigir propriedades adicionais, você deve usar escopos de permissão application.

## <a name="relationships"></a>Relações

| Relação  | Tipo                                                                  | Descrição                                       |
| :------------ | :-------------------------------------------------------------------- | :------------------------------------------------ |
| assignments   | [coleção educationAssignment](../resources/educationassignment.md) | Atribuições que pertencem ao usuário.             |
| classes       | Coleção [educationClass](../resources/educationclass.md)           | Aulas às quais o usuário pertence. Anulável.      |
| schools       | Coleção [educationSchool](../resources/educationschool.md)         | Escolas às quais o usuário pertence. Anulável.      |
| taughtClasses | Coleção [educationClass](../resources/educationclass.md)           | Classes para as quais o usuário é professor.          |
| user          | [user](../resources/user.md)                                          | O usuário do diretório que corresponde a esse usuário. |

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
