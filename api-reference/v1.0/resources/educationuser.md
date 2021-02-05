---
title: Tipo de recurso educationUser
description: Um usuário no sistema. Essa é uma variante específica de educação do usuário com a mesma `id` que o Microsoft Graph retornará do ponto de extremidade `/users` não específico da educação.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9ca45981d2825769f540048a94488dda4ba91c00
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115189"
---
# <a name="educationuser-resource-type"></a>Tipo de recurso educationUser

Namespace: microsoft.graph

Um usuário no sistema. Essa é uma variante específica de educação do usuário com a mesma `id` que o Microsoft Graph retornará do ponto de extremidade `/users` não específico da educação.
Esse objeto fornece um subconjunto direcionado de propriedades do objeto principal [user] e adiciona um conjunto de propriedades específico de educação, como dados de `primaryRole`, aluno e professor.

## <a name="methods"></a>Métodos

| Método                                               | Tipo de retorno                  | Descrição                                                                   |
| :--------------------------------------------------- | :--------------------------- | :---------------------------------------------------------------------------- |
| [Obter educationUser](../api/educationuser-get.md)     | [educationUser]              | Leia as propriedades e relações de um objeto **educationUser**.             |
| [Listar classes](../api/educationuser-list-classes.md) | Coleção [educationClass]  | Obtenha a coleção de objetos **educationClass** da qual o usuário é membro.    |
| [Listar escolas](../api/educationuser-list-schools.md) | Coleção [educationSchool] | Obtenha a coleção de objetos **educationSchool** da qual o usuário é um membro. |
| [Obter usuário](../api/educationuser-get-user.md)         | [user]                       | Obtenha o **user** do diretório simples que corresponde a esse **educationUser**. |
| [Atualizar](../api/educationuser-update.md)             | [educationUser]              | Atualize um objeto **educationUser**.                                           |
| [Delete](../api/educationuser-delete.md)             | Nenhuma                         | Exclua um objeto **educationUser**.                                           |

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo                         | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| :---------------- | :--------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled    | Boolean                      | **True** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                                                    |
| assignedLicenses  | Coleção [assignedLicense] | As licenças que são atribuídas ao usuário. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| assignedPlans     | Coleção [assignedPlan]    | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| businessPhones    | Coleção de cadeias de caracteres            | Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                                                                                                                                                                                                                                                                                                                                                                |
| createdBy         | [identitySet]                | Entidade que criou o usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| department        | String                       | O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| displayName       | String                       | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.                                                                                                                                                                                                                                                           |
| externalSource    | `educationExternalSource`    | De onde esse usuário foi criado. Os valores possíveis são: `sis` , `manual` .                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| givenName         | String                       | O nome fornecido (nome) do usuário. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| id                | String                       | O identificador exclusivo do usuário. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.                                                                                                                                                                                                                                                                                                                                                                                                          |
| email              | String                       | O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mailingAddress    | [physicalAddress]            | Endereço de email do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| mailNickname      | String                       | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                                                                           |
| middleName        | String                       | O nome do meio do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mobilePhone       | String                       | O número de celular principal do usuário.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| passwordPolicies  | String                       | Especifica as políticas de senha do usuário. Este valor é uma enumeração com um possível valor sendo "DisableStrongPassword", que permite especificar as senhas mais fracas do que a política padrão. O "DisablePasswordExpiration" também pode ser especificado. Os dois podem ser especificados juntos, por exemplo: "DisablePasswordExpiration, DisableStrongPassword".                                                                                                                                                                      |
| passwordProfile   | [PasswordProfile]            | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.                                                                                                                                                                                                                             |
| preferredLanguage | String                       | O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo, "en-US".                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| primaryRole       | educationUserRole            | Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student` , `teacher` . Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                             |
| provisionedPlans  | Coleção [ProvisionedPlan] | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| residenceAddress  | [physicalAddress]            | Endereço em que o usuário reside.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| student           | [educationStudent]           | Se a função principal for aluno, esse bloco conterá dados específicos do aluno.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| surname           | String                       | O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| teacher           | [educationTeacher]           | Se a função principal for o professor, esse bloco conterá dados específicos do professor.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| usageLocation     | String                       | Um código de país de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços em países ou regiões. Os exemplos incluem: "US", "JP" e "GB". Não anulável. Oferece suporte a $filter.                                                                                                                                                                                                                                                                |
| userPrincipalName | String                       | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, onde o domínio deve estar presente na coleta de domínios verificados pelo locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). Oferece suporte a $filter e $orderby. |
| userType          | String                       | Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como "Member" e "Guest". Oferece suporte a $filter.                                                                                                                                                                                                                                                                                                                                                                                                        |

## <a name="relationships"></a>Relações

| Relação | Tipo                         | Descrição                                    |
| :----------- | :--------------------------- | :--------------------------------------------- |
| classes      | Coleção [educationClass]  | Aulas às quais o usuário pertence. Anulável.   |
| schools      | Coleção [educationSchool] | Escolas às quais o usuário pertence. Anulável.   |
| assignments  | [educationAssignment]        | Lista de atribuições para o usuário. Anulável.    |
| user         | [usuário]                       | O usuário do diretório correspondente a esse usuário. |

>[!IMPORTANT]
>O **[recurso educationAssignment]** é um recurso de versão /beta. Se for usar esse recurso, não se esqueça de revisar o [log de alterações](/graph/changelog) periodicamente. Quando os recursos da API do Microsoft Graph são lançados para o ponto de extremidade /v1.0, a versão é notada no log de alterações. Se seu aplicativo consumir o **recurso educationAssignment,** você precisará declarar URLs de solicitação base, conforme mostrado no seguinte bloco de código:  
>
>```JavaScript
>var v1BaseUrl = "https://graph.microsoft.com/v1.0/education";
>var betaBaseUrl = "https://graph.microsoft.com/beta/education";  // for administrativeUnit and educationOrganization
>```

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "accountEnabled": true,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["555-555-6568"],
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "preferredLanguage": "string",
  "primaryRole": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"},
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string"
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
      Referenced type microsoft.graph.educationAssignment is not defined in the doc set! Potential suggestion: UNKNOWN",
    "Warning: /api-reference/v1.0/resources/educationuser.md/microsoft.graph.educationUser:
      Property 'relatedContacts' found in markdown table but not in resource definition."
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
[usuário]: user.md
[directoryobject]: directoryobject.md

