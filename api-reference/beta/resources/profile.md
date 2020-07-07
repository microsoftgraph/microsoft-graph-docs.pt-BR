---
title: tipo de recurso Profile
description: Representa propriedades que são descritivas de um usuário e que são mostradas em compartilhamento, as experiências de pessoas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1f80dfccbd662e1e398c0d4b79b0086575a83e2b
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050874"
---
# <a name="profile-resource-type"></a>tipo de recurso Profile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa propriedades que são descritivas de um usuário em um locatário, por exemplo, aniversários e atividades de educação. Essas propriedades são discadas em Shared, experiências de pessoas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph. 

Programaticamente, essas propriedades são expressas como [relações](#relationships) do recurso de **perfil** . Para obter uma destas propriedades de navegação ou criar uma instância dessas propriedades para o usuário, use o método GET ou POST correspondente nessa propriedade, quando aplicável. Consulte os [métodos](#methods) listados abaixo.

## <a name="methods"></a>Métodos

| Método                                                                     | Tipo de retorno                                                    | Descrição                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [Obter perfil](../api/profile-get.md)                                       | [perfil](profile.md)                                          | Leia as propriedades e as relações do objeto de perfil.                                         |
| [Excluir perfil](../api/profile-delete.md)                                 | Nenhum                                                           | Excluir um objeto de **perfil** .                                                                 |
| [Listar conta](../api/profile-list-account.md)                             | coleção [userAccountInformation](useraccountinformation.md) | Obtenha uma coleção de objetos **userAccountInformation** .                                          |
| [Criar personAnniversary](../api/profile-post-anniversaries.md)           | [personAnniversary](personanniversary.md)                      | Crie um novo **personAnniversary** postando na coleção de datas comemorativas.               |
| [Listar aniversários](../api/profile-list-anniversaries.md)                 | coleção [personAnniversary](personanniversary.md)           | Obtenha uma coleção de objetos **personAnniversary** .                                               |
| [Criar educationalActivity](../api/profile-post-educationalactivities.md) | [educationalActivity](educationalactivity.md)                  | Crie um novo **educationalActivity** postando na coleção **educationalActivities** . |
| [Listar educationalActivities](../api/profile-list-educationalactivities.md) | coleção [educationalActivity](educationalactivity.md)       | Obtenha uma coleção de objetos **educationalActivity** .                                            |
| [Criar email](../api/profile-post-emails.md)                          | [Email](itememail.md)                                      | Crie um novo **email** postando na coleção emails.                              |
| [Listar emails](../api/profile-list-emails.md)                               | coleção [email](itememail.md)                           | Obter uma coleção de objetos de **email** .                                                      |
| [Criar personInterest](../api/profile-post-interests.md)                  | [personInterest](personinterest.md)                            | Crie um novo **personInterest** postando na coleção interesses.                      |
| [Listar interesses](../api/profile-list-interests.md)                         | coleção [personInterest](personinterest.md)                 | Obtenha uma coleção de objetos **personInterest** .                                                  |
| [Criar languageProficiency](../api/profile-post-languages.md)             | [languageProficiency](languageproficiency.md)                  | Crie um novo **languageProficiency** postando na coleção de idiomas.                 |
| [Idiomas de lista](../api/profile-list-languages.md)                         | coleção [languageProficiency](languageproficiency.md)       | Obtenha uma coleção de objetos **languageProficiency** .                                             |
| [Nomes da lista](../api/profile-list-names.md)                                 | coleção [PersonName](personname.md)                         | Obtenha uma coleção de objetos **PersonName** .                                                      |
| [Criar PersonName](../api/profile-post-names.md)                          | [personName](personName.md)                                    | Crie um novo objeto **PersonName** postando na coleção names.                       |
| [Listar sites](../api/profile-list-websites.md)                           | coleção [personWebsite](personwebsite.md)                   | Obtenha uma coleção de objetos **personWebsite** .                                                   |
| [Criar um número de telefone](../api/profile-post-phones.md)                          | [Número de telefone](itemphone.md)                                      | Criar um novo meu telefone postando na coleção phones.                                  |
| [Listar telefones](../api/profile-list-phones.md)                               | coleção [Multiphone](itemphone.md)                           | Obter uma coleção de objetos de **Multiphone** .                                                       |
| [Criar workPosition](../api/profile-post-positions.md)                    | [workPosition](workposition.md)                                | Crie um novo workPosition postando na coleção Positions.                            |
| [Listar posições](../api/profile-list-positions.md)                         | coleção [workPosition](workposition.md)                     | Obtenha uma coleção de objetos **workPosition** .                                                    |
| [Criar projectParticipation](../api/profile-post-projects.md)             | [projectParticipation](projectparticipation.md)                | Criar um novo **projectParticipation** postando na coleção Projects.                 |
| [Listar projetos](../api/profile-list-projects.md)                           | coleção [projectParticipation](projectparticipation.md)     | Obtenha uma coleção de objetos **projectParticipation** .                                            |
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
|Count                |coleção [userAccountInformation](useraccountinformation.md)| Representa informações especificamente associadas à conta de um usuário. Somente leitura. Anulável.                                                             |
|datas especiais          |coleção [personAnniversary](personanniversary.md)          | Representa os detalhes de datas significativas associadas a uma pessoa. Somente leitura. Anulável.                                                      |
|educationalActivities  |coleção [educationalActivity](educationalactivity.md)      | Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais. Somente leitura. Anulável.|
|email                 |coleção [email](itememail.md)                          | Representa informações detalhadas sobre endereços de email associados ao usuário. Somente leitura. Anulável.                                           |
|interests              |coleção [personInterest](personinterest.md)                | Fornece informações detalhadas sobre os interesses que o usuário tenha associado a si mesmos em vários serviços. Somente leitura. Anulável.                |
|Idiomas              |coleção [languageProficiency](languageproficiency.md)      | Representa informações detalhadas sobre os idiomas que um usuário adicionou ao perfil. Somente leitura. Anulável.                                   |
|telefones                 |coleção [Multiphone](itemphone.md)                          | Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços. Somente leitura. Anulável.                           |
|as              |coleção [workPosition](workposition.md)                    | Representa informações detalhadas sobre posições de trabalho associadas ao perfil de um usuário. Somente leitura. Anulável.                                    |
|Projetos               |coleção [projectParticipation](projectparticipation.md)    | Representa informações detalhadas sobre os projetos associados a um usuário. Somente leitura. Anulável.                                                    |
|skills                 |coleção [skillProficiency](skillproficiency.md)            | Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços. Somente leitura. Anulável.                                  |
|contas da            |coleção [Webaccount](webaccount.md)                        | Representa contas da Web que o usuário indicou que usa ou adicionou ao perfil do usuário. Somente leitura. Anulável.                               |
|websites               |coleção [personWebsite](personwebsite.md)                  | Representa informações detalhadas sobre sites associados a um usuário em vários serviços. Somente leitura. Anulável.                                |

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

<!--
{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
-->


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
