---
title: tipo de recurso Profile
description: Representa propriedades que são descritivas de um usuário e que são mostradas em compartilhamento, as experiências de pessoas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4080a7424b1ee3baf71cfaab3cf3e66a8f0508b6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810514"
---
# <a name="profile-resource-type"></a>tipo de recurso Profile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa propriedades que são descritivas de um usuário em um locatário, por exemplo, aniversários e atividades de educação. Essas propriedades são discadas em Shared, experiências de pessoas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph. 

Programaticamente, essas propriedades são expressas como [relações](#relationships) do recurso de **perfil** . Para obter uma destas propriedades de navegação ou criar uma instância dessas propriedades para o usuário, use o método GET ou POST correspondente nessa propriedade, quando aplicável. Consulte os [métodos](#methods) listados abaixo.

## <a name="methods"></a>Métodos

| Método                                                                     | Tipo de retorno                                                    | Descrição                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [Obter perfil](../api/profile-get.md)                                       | [perfil](profile.md)                                          | Leia as propriedades e as relações do objeto de perfil.                                     |
| [Excluir perfil](../api/profile-delete.md)                                 | Nenhum                                                           | Excluir um objeto de **perfil** .                                                                 |
| [Criar userAccountInformation](../api/profile-post-accounts.md)           | [userAccountInformation](useraccountinformation.md)            | Criar um novo objeto **userAccountInformation** postando na coleção accounts.        |
| [Listar contas](../api/profile-list-accounts.md)                           | coleção [userAccountInformation](useraccountinformation.md) | Obtenha uma coleção de objetos **userAccountInformation** .                                          |
| [Criar endereço](../api/profile-post-addresses.md)                     | [Endereço do destinatário](itemaddress.md)                                  | Crie um novo **endereço** postando na coleção addresses.                         |
| [Listar endereços](../api/profile-list-addresses.md)                         | coleção [myAddress](itemaddress.md)                       | Obtenha uma coleção de objetos de **endereço** .                                                    |
| [Criar personAnniversary](../api/profile-post-anniversaries.md)           | [personAnniversary](personanniversary.md)                      | Crie um novo **personAnniversary** postando na coleção de datas comemorativas.               |
| [Listar aniversários](../api/profile-list-anniversaries.md)                 | coleção [personAnniversary](personanniversary.md)           | Obtenha uma coleção de objetos **personAnniversary** .                                               |
| [Criar personAward](../api/profile-post-awards.md)                        | [personAward](personaward.md)                                  | Criar um novo objeto **personAward** postando na coleção de prêmios.                     |
| [Listar prêmios](../api/profile-list-awards.md)                               | coleção [personAward](personaward.md)                       | Obtenha uma coleção de objetos **personAward** .                                                     |
| [Criar personCertification](../api/profile-post-certifications.md)        | [personCertification](personcertification.md)                  | Criar um novo objeto **personCertification** postando na coleção certificações.     |
| [Listar certificações](../api/profile-list-certifications.md)               | coleção [personCertification](personcertification.md)       | Obtenha uma coleção de objetos **personCertification** .                                             |
| [Criar educationalActivity](../api/profile-post-educationalactivities.md) | [educationalActivity](educationalactivity.md)                  | Crie um novo **educationalActivity** postando na coleção **educationalActivities** . |
| [Listar educationalActivities](../api/profile-list-educationalactivities.md) | coleção [educationalActivity](educationalactivity.md)       | Obtenha uma coleção de objetos **educationalActivity** .                                            |
| [Criar email](../api/profile-post-emails.md)                          | [Email](itememail.md)                                      | Crie um novo **email** postando na coleção emails.                              |
| [Listar emails](../api/profile-list-emails.md)                               | coleção [email](itememail.md)                           | Obter uma coleção de objetos de **email** .                                                      |
| [Criar personInterest](../api/profile-post-interests.md)                  | [personInterest](personinterest.md)                            | Crie um novo **personInterest** postando na coleção interesses.                      |
| [Listar interesses](../api/profile-list-interests.md)                         | coleção [personInterest](personinterest.md)                 | Obtenha uma coleção de objetos **personInterest** .                                                  |
| [Criar languageProficiency](../api/profile-post-languages.md)             | [languageProficiency](languageproficiency.md)                  | Crie um novo **languageProficiency** postando na coleção de idiomas.                 |
| [Idiomas de lista](../api/profile-list-languages.md)                         | coleção [languageProficiency](languageproficiency.md)       | Obtenha uma coleção de objetos **languageProficiency** .                                             |
| [Criar PersonName](../api/profile-post-names.md)                          | [personName](personname.md)                                    | Crie um novo objeto **PersonName** postando na coleção names.                       |
| [Nomes da lista](../api/profile-list-names.md)                                 | coleção [PersonName](personname.md)                         | Obtenha uma coleção de objetos **PersonName** .                                                      |
| [Criar personAnnotation](../api/profile-post-notes.md)                    | [personAnnotation](personannotation.md)                        | Criar um novo objeto **personAnnotation** postando na coleção Notes.                 |
| [Listar anotações](../api/profile-list-notes.md)                                 | coleção [personAnnotation](personannotation.md)             | Obtenha uma coleção de objetos **personAnnotation** .                                                |
| [Criar ispatente](../api/profile-post-patents.md)                        | [Patente](itempatent.md)                                    | Crie um novo objeto de **patente** postando na coleção de patentes.                     |
| [Listar patentes](../api/profile-list-patents.md)                             | coleção [Ispatenteado](itempatent.md)                         | Obter uma coleção de objetos de **ispatente** .                                                      |
| [Criar um número de telefone](../api/profile-post-phones.md)                          | [Número de telefone](itemphone.md)                                      | Criar um novo meu telefone postando na coleção phones.                                  |
| [Listar telefones](../api/profile-list-phones.md)                               | coleção [Multiphone](itemphone.md)                           | Obter uma coleção de objetos de **Multiphone** .                                                       |
| [Criar workPosition](../api/profile-post-positions.md)                    | [workPosition](workposition.md)                                | Crie um novo workPosition postando na coleção Positions.                            |
| [Listar posições](../api/profile-list-positions.md)                         | coleção [workPosition](workposition.md)                     | Obtenha uma coleção de objetos **workPosition** .                                                    |
| [Criar projectParticipation](../api/profile-post-projects.md)             | [projectParticipation](projectparticipation.md)                | Criar um novo **projectParticipation** postando na coleção Projects.                 |
| [Listar projetos](../api/profile-list-projects.md)                           | coleção [projectParticipation](projectparticipation.md)     | Obtenha uma coleção de objetos **projectParticipation** .                                            |
| [Criar a multipúblico](../api/profile-post-publications.md)              | [multipúblico](itempublication.md)                          | Crie **um novo objeto de publicação** postando na coleção de publicações.           |
| [Listar publicações](../api/profile-list-publications.md)                   | coleção de [Multipúblico](itempublication.md)               | Obtenha uma coleção de objetos de **multipúblico** .                                                 |
| [Criar personResponsibility](../api/profile-post-responsibilities.md)     | [personResponsibility](personresponsibility.md)                | Criar um novo objeto **personResponsibility** postando na coleção responsabilidades.  |
| [Listar responsabilidades](../api/profile-list-responsibilities.md)           | coleção [personResponsibility](personresponsibility.md)     | Obtenha uma coleção de objetos **personResponsibility** .                                            |
| [Criar skillProficiency](../api/profile-post-skills.md)                   | [skillProficiency](skillproficiency.md)                        | Crie um novo **skillProficiency** postando na coleção de habilidades.                       |
| [Listar qualificações](../api/profile-list-skills.md)                               | coleção [skillProficiency](skillproficiency.md)             | Obtenha uma coleção de objetos **skillProficiency** .                                                |
| [Criar conta da](../api/profile-post-webaccounts.md)                    | [conta da](webaccount.md)                                    | Crie uma nova **conta da webaccount** postando na coleção webaccounts.                        |
| [Listar contas da webaccount](../api/profile-list-webaccounts.md)                     | coleção [Webaccount](webaccount.md)                         | Obtenha uma coleção de objetos **webaccount** .                                                      |
| [Criar personWebsite](../api/profile-post-websites.md)                    | [personWebsite](personwebsite.md)                              | Crie um novo **personWebsite** postando na coleção sites.                        |
| [Listar sites](../api/profile-list-websites.md)                           | coleção [personWebsite](personwebsite.md)                   | Obtenha uma coleção de objetos **personWebsite** .                                                   |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id            |String       | Somente leitura.  |

## <a name="relationships"></a>Relações

| Relação          | Tipo                                                         | Descrição                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|contas               |coleção [userAccountInformation](useraccountinformation.md)| Representa informações especificamente associadas à conta de um usuário.                                                             |
|endereços              |coleção [myAddress](itemaddress.md)                      | Representa detalhes dos endereços associados ao usuário.                                                             |
|datas especiais          |coleção [personAnniversary](personanniversary.md)          | Representa os detalhes de datas significativas associadas a uma pessoa.                                                                  |
|concede                 |coleção [personAward](personaward.md)                      | Representa os detalhes de prêmios ou honras associados a uma pessoa.                                                                  |
|certificações         |coleção [personCertification](personcertification.md)      | Representa os detalhes de certificações associadas a uma pessoa.                                                                  |
|educationalActivities  |coleção [educationalActivity](educationalactivity.md)      | Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais. |
|email                 |coleção [email](itememail.md)                          | Representa informações detalhadas sobre endereços de email associados ao usuário.                       |
|interests              |coleção [personInterest](personinterest.md)                | Fornece informações detalhadas sobre os interesses que o usuário tenha associado a si mesmos em vários serviços.             |
|Idiomas              |coleção [languageProficiency](languageproficiency.md)      | Representa informações detalhadas sobre os idiomas que um usuário adicionou ao perfil.                                    |
|names                  |coleção [PersonName](personname.md)                        | Representa os nomes que um usuário adicionou ao perfil.                                    |
|notes                  |coleção [personAnnotation](personannotation.md)            | Representa as anotações que um usuário adicionou ao seu perfil.                                    |
|patentes                |coleção [Ispatenteado](itempatent.md)                        | Representa patentes que um usuário adicionou ao seu perfil.                                    |
|telefones                 |coleção [Multiphone](itemphone.md)                          | Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.                            |
|as              |coleção [workPosition](workposition.md)                    | Representa informações detalhadas sobre posições de trabalho associadas ao perfil de um usuário.                                    |
|Projetos               |coleção [projectParticipation](projectparticipation.md)    | Representa informações detalhadas sobre os projetos associados a um usuário.                                                     |
|publicações           |coleção de [Multipúblico](itempublication.md)              | Representa os detalhes de todas as publicações adicionadas por um usuário ao seu perfil.                                                     |
|responsibilities       |coleção [personResponsibility](personResponsibility.md)    | Representa detalhes das responsabilidades adicionadas por um usuário ao seu perfil.                                                     |
|skills                 |coleção [skillProficiency](skillproficiency.md)            | Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.                                   |
|contas da            |coleção [Webaccount](webaccount.md)                        | Representa contas da Web que o usuário indicou que usa ou adicionou ao perfil do usuário.                               |
|websites               |coleção [personWebsite](personwebsite.md)                  | Representa informações detalhadas sobre sites associados a um usuário em vários serviços.                                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "String (identifier)"
}
```
