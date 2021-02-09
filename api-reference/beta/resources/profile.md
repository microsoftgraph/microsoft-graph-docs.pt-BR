---
title: tipo de recurso de perfil
description: Representa propriedades descritivas de um usuário e que são apresentados em experiências compartilhadas de pessoas no Microsoft 365 e em serviços e experiências de terceiros por meio do Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 542d5907bd1bc467c32ae58836df04a2c62df36f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153512"
---
# <a name="profile-resource-type"></a>tipo de recurso de perfil

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa propriedades que são descritivas de um usuário em um locatário, por exemplo, aniversários e atividades de educação. Essas propriedades são fornecidas em experiências compartilhadas e de pessoas no Microsoft 365 e em experiências e serviços de terceiros por meio do Microsoft Graph. 

Programaticamente, essas propriedades são [expressas como relações do](#relationships) recurso **de** perfil. Para obter uma dessas propriedades de navegação ou criar uma instância dessas propriedades para o usuário, use o método GET ou POST correspondente nessa propriedade, quando aplicável. Consulte os [métodos listados](#methods) abaixo.

## <a name="methods"></a>Métodos

| Método                                                                     | Tipo de retorno                                                    | Descrição                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [Obter perfil](../api/profile-get.md)                                       | [perfil](profile.md)                                          | Leia as propriedades e as relações do objeto de perfil.                                     |
| [Excluir perfil](../api/profile-delete.md)                                 | Nenhum                                                           | Exclua **um objeto de** perfil.                                                                 |
| [Criar userAccountInformation](../api/profile-post-accounts.md)           | [userAccountInformation](useraccountinformation.md)            | Crie um novo **objeto userAccountInformation** postando na coleção de contas.        |
| [Listar contas](../api/profile-list-accounts.md)                           | [Coleção userAccountInformation](useraccountinformation.md) | Obter uma **coleção de objetos userAccountInformation.**                                          |
| [Criar itemAddress](../api/profile-post-addresses.md)                     | [itemAddress](itemaddress.md)                                  | Crie um novo **itemAddress** postando na coleção addresses.                         |
| [Endereços de lista](../api/profile-list-addresses.md)                         | [Coleção itemAddress](itemaddress.md)                       | Obter uma **coleção de objetos itemAddress.**                                                    |
| [Criar personAnniversary](../api/profile-post-anniversaries.md)           | [personAnniversary](personanniversary.md)                      | Crie um **novo personAnniversary** postando na coleção anniversaries.               |
| [Listar anniversaries](../api/profile-list-anniversaries.md)                 | [Coleção personAnniversary](personanniversary.md)           | Obter uma **coleção de objetos personAnniversary.**                                               |
| [Criar personAward](../api/profile-post-awards.md)                        | [personAward](personaward.md)                                  | Crie um novo **objeto personAward** postando na coleção Awards.                     |
| [Listar prêmio](../api/profile-list-awards.md)                               | [coleção personAward](personaward.md)                       | Obter uma **coleção de objetos personAward.**                                                     |
| [Criar personCertification](../api/profile-post-certifications.md)        | [personCertification](personcertification.md)                  | Crie um novo **objeto personCertification** postando na coleção certifications.     |
| [Listar certificações](../api/profile-list-certifications.md)               | [Coleção personCertification](personcertification.md)       | Obter uma **coleção de objetos personCertification.**                                             |
| [Criar educationalActivity](../api/profile-post-educationalactivities.md) | [educationalActivity](educationalactivity.md)                  | Crie uma nova **educationalActivity** postando na **coleção educationalActivities.** |
| [Listar educationalActivities](../api/profile-list-educationalactivities.md) | [coleção educationalActivity](educationalactivity.md)       | Obter uma **coleção de objetos educationalActivity.**                                            |
| [Criar itemEmail](../api/profile-post-emails.md)                          | [itemEmail](itememail.md)                                      | Crie um novo **itemEmail** postando na coleção de emails.                              |
| [Listar emails](../api/profile-list-emails.md)                               | [coleção itemEmail](itememail.md)                           | Obter uma **coleção de objetos itemEmail.**                                                      |
| [Criar personInterest](../api/profile-post-interests.md)                  | [personInterest](personinterest.md)                            | Crie um novo **personInterest** postando na coleção de interesses.                      |
| [Listar interesses](../api/profile-list-interests.md)                         | [Coleção personInterest](personinterest.md)                 | Obter uma **coleção de objetos personInterest.**                                                  |
| [Criar languageProficiency](../api/profile-post-languages.md)             | [languageProficiency](languageproficiency.md)                  | Crie uma **nova languageProficiency** postando na coleção de idiomas.                 |
| [Idiomas da lista](../api/profile-list-languages.md)                         | [Coleção languageProficiency](languageproficiency.md)       | Obter uma **coleção de objetos languageProficiency.**                                             |
| [Criar personName](../api/profile-post-names.md)                          | [personName](personname.md)                                    | Crie um novo **objeto personName** postando na coleção names.                       |
| [Nomes da lista](../api/profile-list-names.md)                                 | [Coleção personName](personname.md)                         | Obter uma **coleção de objetos personName.**                                                      |
| [Criar personAnnotation](../api/profile-post-notes.md)                    | [personAnnotation](personannotation.md)                        | Crie um novo **objeto personAnnotation** postando na coleção de anotações.                 |
| [Listar anotações](../api/profile-list-notes.md)                                 | [Coleção personAnnotation](personannotation.md)             | Obter uma **coleção de objetos personAnnotation.**                                                |
| [Criar itemPatent](../api/profile-post-patents.md)                        | [itemPatent](itempatent.md)                                    | Crie um novo **objeto itemPatent** postando na coleção patents.                     |
| [Listar patentes](../api/profile-list-patents.md)                             | [Coleção itemPatent](itempatent.md)                         | Obter uma **coleção de objetos itemPatent.**                                                      |
| [Criar itemPhone](../api/profile-post-phones.md)                          | [itemPhone](itemphone.md)                                      | Crie um novo itemPhone postando na coleção phones.                                  |
| [Listar telefones](../api/profile-list-phones.md)                               | [Coleção itemPhone](itemphone.md)                           | Obter uma **coleção de objetos itemPhone.**                                                       |
| [Criar workPosition](../api/profile-post-positions.md)                    | [workPosition](workposition.md)                                | Crie uma nova workPosition postando na coleção positions.                            |
| [Listar posições](../api/profile-list-positions.md)                         | [coleção workPosition](workposition.md)                     | Obter uma **coleção de objetos workPosition.**                                                    |
| [Criar projectParticipation](../api/profile-post-projects.md)             | [projectParticipation](projectparticipation.md)                | Crie um novo **projectParticipation** postando na coleção de projetos.                 |
| [Listar projetos](../api/profile-list-projects.md)                           | [coleção projectParticipation](projectparticipation.md)     | Obter uma **coleção de objetos projectParticipation.**                                            |
| [Criar itemPublication](../api/profile-post-publications.md)              | [itemPublication](itempublication.md)                          | Crie um novo **objeto itemPublication** postando na coleção de publicações.           |
| [Listar publicações](../api/profile-list-publications.md)                   | [coleção itemPublication](itempublication.md)               | Obter uma **coleção de objetos itemPublication.**                                                 |
| [Criar personResponsibility](../api/profile-post-responsibilities.md)     | [personResponsibility](personresponsibility.md)                | Crie um novo **objeto personResponsibility** postando na coleção responsibilities.  |
| [Listar responsabilidades](../api/profile-list-responsibilities.md)           | [coleção personResponsibility](personresponsibility.md)     | Obter uma **coleção de objetos personResponsibility.**                                            |
| [Criar skillProficiency](../api/profile-post-skills.md)                   | [skillProficiency](skillproficiency.md)                        | Crie uma **nova habilidade postando** na coleção de habilidades.                       |
| [Listar habilidades](../api/profile-list-skills.md)                               | [Coleção skillProficiency](skillproficiency.md)             | Obter uma **coleção de objetos skillProficiency.**                                                |
| [Criar webAccount](../api/profile-post-webaccounts.md)                    | [webAccount](webaccount.md)                                    | Crie uma nova **webAccount** postando na coleção webAccounts.                        |
| [Listar webAccounts](../api/profile-list-webaccounts.md)                     | [coleção webAccount](webaccount.md)                         | Obter uma **coleção de objetos webAccount.**                                                      |
| [Criar personWebsite](../api/profile-post-websites.md)                    | [personWebsite](personwebsite.md)                              | Crie um novo **personWebsite** postando na coleção de sites.                        |
| [Listar sites](../api/profile-list-websites.md)                           | [coleção personWebsite](personwebsite.md)                   | Obter uma **coleção de objetos personWebsite.**                                                   |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id            |String       | Somente leitura.  |

## <a name="relationships"></a>Relações

| Relação          | Tipo                                                         | Descrição                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|contas               |[Coleção userAccountInformation](useraccountinformation.md)| Representa informações especificamente vinculadas à conta de um usuário.                                                             |
|addresses              |[Coleção itemAddress](itemaddress.md)                      | Representa detalhes dos endereços associados ao usuário.                                                             |
|anniversaries          |[Coleção personAnniversary](personanniversary.md)          | Representa os detalhes de datas significativas associadas a uma pessoa.                                                                  |
|awards                 |[coleção personAward](personaward.md)                      | Representa os detalhes dos prêmio ou das entidades associadas a uma pessoa.                                                                  |
|certifications         |[Coleção personCertification](personcertification.md)      | Representa os detalhes das certificações associadas a uma pessoa.                                                                  |
|educationalActivities  |[coleção educationalActivity](educationalactivity.md)      | Representa os dados que um usuário forneceu relacionados à inigressão, à responsabilidade, à instituição de ensino ou a outras atividades educacionais. |
|emails                 |[coleção itemEmail](itememail.md)                          | Representa informações detalhadas sobre endereços de email associados ao usuário.                       |
|interests              |[Coleção personInterest](personinterest.md)                | Fornece informações detalhadas sobre os interesses que o usuário associou a si mesmo em vários serviços.             |
|idiomas              |[Coleção languageProficiency](languageproficiency.md)      | Representa informações detalhadas sobre idiomas que um usuário adicionou ao seu perfil.                                    |
|names                  |[coleção personName](personname.md)                        | Representa os nomes que um usuário adicionou ao seu perfil.                                    |
|notes                  |[Coleção personAnnotation](personannotation.md)            | Representa anotações que um usuário adicionou ao seu perfil.                                    |
|patents                |[Coleção itemPatent](itempatent.md)                        | Representa patentes que um usuário adicionou ao seu perfil.                                    |
|telefones                 |[Coleção itemPhone](itemphone.md)                          | Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.                            |
|positions              |[coleção workPosition](workposition.md)                    | Representa informações detalhadas sobre as posições de trabalho associadas ao perfil de um usuário.                                    |
|Projetos               |[coleção projectParticipation](projectparticipation.md)    | Representa informações detalhadas sobre projetos associados a um usuário.                                                     |
|publications           |[coleção itemPublication](itempublication.md)              | Representa detalhes de quaisquer publicações que um usuário tenha adicionado ao seu perfil.                                                     |
|responsibilities       |[coleção personResponsibility](personResponsibility.md)    | Representa os detalhes das responsabilidades que um usuário adicionou ao seu perfil.                                                     |
|skills                 |[Coleção skillProficiency](skillproficiency.md)            | Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.                                   |
|webAccounts            |[coleção webAccount](webaccount.md)                        | Representa contas da Web que o usuário indicou que usa ou adicionou ao seu perfil de usuário.                               |
|websites               |[coleção personWebsite](personwebsite.md)                  | Representa informações detalhadas sobre sites associados a um usuário em vários serviços.                                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "keyProperty": "id"
}-->

```json
{
    "id": "String (identifier)"
}
```


