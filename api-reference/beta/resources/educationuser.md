---
title: Tipo de recurso educationUser
description: Um usuário no sistema. Essa é uma variante específica de educação do usuário com a mesma `id` que o Microsoft Graph retornará do ponto de extremidade `/users` não específico da educação.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 71716936fcbdf3f820feafeef84498ebbe4ff422
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909699"
---
# <a name="educationuser-resource-type"></a>Tipo de recurso educationUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um usuário no sistema. Esta é uma variante específica da educação do recurso [usuário] padrão, com o mesmo `id` que o Microsoft Graph retornará do ponto de extremidade não específico da educação `/users` .

Este objeto fornece um subconjunto direcionado de propriedades do objeto de [usuário] principal e adiciona um conjunto de propriedades específicas de educação, como `primaryRole` , `student` e `teacher` .

## <a name="methods"></a>Métodos

| Método                                               | Tipo de retorno                                  | Descrição                                                                   |
| :--------------------------------------------------- | :------------------------------------------- | :---------------------------------------------------------------------------- |
| [Obter educationUser](../api/educationuser-get.md)     | [educationUser]                              | Leia as propriedades e relações de um objeto **educationUser**.             |
| [Listar classes](../api/educationuser-list-classes.md) | Coleção [educationClass]                  | Obtenha a coleção de objetos **educationClass** da qual o usuário é membro.    |
| [Listar escolas](../api/educationuser-list-schools.md) | Coleção [educationSchool]                 | Obtenha a coleção de objetos **educationSchool** da qual o usuário é um membro. |
| [Obter usuário](../api/educationuser-get-user.md)         | [user]                                       | Obtenha o **user** do diretório simples que corresponde a esse **educationUser**. |
| [Atualizar](../api/educationuser-update.md)             | [educationUser]                              | Atualize um objeto **educationUser**.                                           |
| [Delete](../api/educationuser-delete.md)             | Nenhum                                         | Exclua um objeto **educationUser**.                                           |
| [Delta](../api/educationuser-delta.md)               | Coleção [educationUser](educationuser.md) | Obter alterações incrementais para o **educationUsers**.                               |

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo                         | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| :---------------- | :--------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                | String                       | O identificador exclusivo do usuário. Herdado de [directoryObject]. Chave. Não anulável. Somente leitura.                                                                                                                                                                                                                                                                                                                                                                                                                              |
| accountEnabled    | Booliano                      | **True** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                                                                                                                                                                   |
| assignedLicenses  | Coleção [assignedLicense] | As licenças que são atribuídas ao usuário. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| assignedPlans     | Coleção [assignedPlan]    | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| businessPhones    | Coleção de cadeias de caracteres            | Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                                                                                                                                                                                                                                                                                                                                                                |
| createdBy         | [identitySet]                | Entidade que criou o usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| department        | String                       | O nome do departamento no qual o usuário trabalha. Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| displayName       | Cadeia de caracteres                       | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.                                                                                                                                                                                                                                                           |
| externalSource    | String                       | De onde esse usuário foi criado. Os valores possíveis são: `sis` , `lms` , ou `manual` .                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| givenName         | String                       | O nome fornecido (nome) do usuário. Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| email              | String                       | O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                                                                                                                                                                                        |
| mailNickname      | String                       | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                                                                                                                                                                                          |
| mailingAddress    | [physicalAddress]            | Endereço de email do usuário. Observação: `type` e `postOfficeBox` não têm suporte para `educationUser` recursos.                                                                                                                                                                                                                                                                                                                                                                                                                          |
| middleName        | String                       | O nome do meio do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mobilePhone       | String                       | O número de celular principal do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| onPremisesInfo    | [educationOnPremisesInfo]    | Informações adicionais usadas para associar o usuário do AAD ao seu equivalente do Active Directory.                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| passwordPolicies  | String                       | Especifica as políticas de senha do usuário. Esse valor é uma enumeração com um valor possível como "DisableStrongPassword", que permite senhas mais fracas do que a política padrão a ser especificada. "DisablePasswordExpiration" também pode ser especificado. Os dois podem ser especificados juntos, por exemplo: "DisablePasswordExpiration, DisableStrongPassword".                                                                                                                                                                      |
| passwordProfile   | [passwordProfile]            | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.                                                                                                                                                                                                                             |
| preferredLanguage | String                       | O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo, "en-US".                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| primaryRole       | cadeia de caracteres                       | Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student`, `teacher`, `faculty`. Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                                                                                                                                     |
| provisionedPlans  | coleção [provisionedPlan] | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| relatedContacts   | coleção [relatedContact]  | Registros relacionados relacionados ao usuário. As relações possíveis `parent` são `relative` , `aide` , `doctor` , `guardian` `child` ,, `other` ,`unknownFutureValue`                                                                                                                                                                                                                                                                                                                                                                       |
| residenceAddress  | [physicalAddress]            | Endereço em que o usuário reside. Observação: `type` e `postOfficeBox` não têm suporte para `educationUser` recursos.                                                                                                                                                                                                                                                                                                                                                                                                                      |
| student           | [educationStudent]           | Se a função principal for aluno, esse bloco conterá dados específicos do aluno.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| surname           | String                       | O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| teacher           | [educationTeacher]           | Se a função principal for professor, esse bloco conterá dados específicos do professor.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| usageLocation     | Cadeia de caracteres                       | Um código de país de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços em países ou regiões. Os exemplos incluem: "US", "JP" e "GB". Não anulável. Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                               |
| userPrincipalName | Cadeia de caracteres                       | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, onde domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). Oferece suporte a $filter e $orderby. |
| userType          | String                       | Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Membro” e “Convidado”. Oferece suporte a \$ filtro.                                                                                                                                                                                                                                                                                                                                                                                                       |

> [!IMPORTANT]
> Ao usar escopos de permissão delegada, o Graph só retornará um conjunto limitado de propriedades:,,,,,,, `id` `primaryRole` ,, `accountEnabled` `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` , `teacher/externalId` . Se seu aplicativo exigir propriedades adicionais, você deve usar escopos de permissão de aplicativo.

## <a name="relationships"></a>Relações

| Relação  | Tipo                         | Descrição                                  |
| :------------ | :--------------------------- | :------------------------------------------- |
| assignments   | [educationAssignment]        | Lista de atribuições para o usuário. Anulável.  |
| classes       | Coleção [educationClass]  | Aulas às quais o usuário pertence. Anulável. |
| schools       | Coleção [educationSchool] | Escolas às quais o usuário pertence. Anulável. |
| taughtClasses | Coleção [educationClass]  | Classes para as quais o usuário é um professor.     |

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
    "Error: Resource educationUser has documented navigation properties, but we thought it was a complex type!"
  ]

}-->

[educationuser]: educationuser.md
[educationclass]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: educationassignment.md
[educationteacher]: educationteacher.md
[educationstudent]: educationstudent.md
[relatedcontact]: relatedcontact.md
[PhysicalAddress]: physicaladdress.md
[provisionedplan]: provisionedplan.md
[passwordprofile]: passwordprofile.md
[identityset]: identityset.md
[assignedplan]: assignedplan.md
[assignedlicense]: assignedlicense.md
[user]: user.md
[directoryobject]: directoryobject.md
[educationonpremisesinfo]: educationonpremisesinfo.md
