---
title: Usar a API de Perfil no Microsoft Graph para recuperar informações sobre determinado usuário ou sobre você mesmo
description: 'Os aplicativos do Microsoft Graph podem usar a API do Perfil para recuperar o perfil de outro usuário. '
author: kevinbellinger
localization_priority: Priority
ms.prod: people
doc_type: conceptualPageType
ms.openlocfilehash: 342eb433f7acc5c8e37d37e7ebcf7cb59f768aa1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939247"
---
# <a name="use-the-profile-api-in-microsoft-graph-to-retrieve-information-about-yourself-or-another-user"></a><span data-ttu-id="19b91-103">Use a API do Perfil no Microsoft Graph para recuperar informações sobre você mesmo ou outro usuário</span><span class="sxs-lookup"><span data-stu-id="19b91-103">Use the Profile API in Microsoft Graph to retrieve information about yourself or another user</span></span> 

<span data-ttu-id="19b91-104">Os aplicativos do Microsoft Graph podem usar a API de Perfil para recuperar o perfil do usuário conectado com uma conta válida do Azure AD ou da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19b91-104">Microsoft Graph applications can use the Profile API to retrieve the profile of the signed-in user or another user with a valid Azure AD or Microsoft account.</span></span> <span data-ttu-id="19b91-105">Essas informações podem ser usadas em aplicativos para ajudar a contextualizar outros usuários, fornecer uma experiência mais avançada para o usuário no aplicativo ou como um mecanismo para armazenar informações estendidas sobre o usuário, as quais também poderão ser usadas no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="19b91-105">This information can be used in applications to assist in contextualizing another user, providing a richer experience for the user within the application or as a mechanism for storing extended information about the user which can also be used within Microsoft 365.</span></span> 

## <a name="authorization"></a><span data-ttu-id="19b91-106">Autorização</span><span class="sxs-lookup"><span data-stu-id="19b91-106">Authorization</span></span>

<span data-ttu-id="19b91-107">Para chamar a API de Pessoas no Microsoft Graph, seu aplicativo precisará das permissões adequadas:</span><span class="sxs-lookup"><span data-stu-id="19b91-107">To call the People API in Microsoft Graph, your app will need the appropriate permissions:</span></span>

* <span data-ttu-id="19b91-108">User.Read – Use para fazer chamadas gerais para a API do Perfil; por exemplo, `https://graph.microsoft.com/beta/me/profile/`.</span><span class="sxs-lookup"><span data-stu-id="19b91-108">People.Read - Use to make general People API calls; for example, `https://graph.microsoft.com/beta/me/profile/`. People.Read requires end user consent.</span></span> <span data-ttu-id="19b91-109">User.Read requer o consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="19b91-109">User.Read requires end user consent.</span></span>

## <a name="view-my-profile"></a><span data-ttu-id="19b91-110">Visualizar meu perfil</span><span class="sxs-lookup"><span data-stu-id="19b91-110">View my profile</span></span>

<span data-ttu-id="19b91-111">As solicitações nesta seção obtém as pessoas mais relevantes para o usuário conectado (`/me`).</span><span class="sxs-lookup"><span data-stu-id="19b91-111">The requests in this section get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="19b91-112">Essas solicitações exigem que a permissão User.Read esteja presente para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="19b91-112">These requests require the User.Read permission to be present for the signed-in user.</span></span> 


```http
GET https://graph.microsoft.com/beta/me/profile/
```

<span data-ttu-id="19b91-p104">O exemplo a seguir mostra a resposta. Por padrão, cada resposta retorna 10 registros. Você pode alterar isso usando o parâmetro de consulta *$top*. Este exemplo usa *$top* para limitar a resposta a três registros.</span><span class="sxs-lookup"><span data-stu-id="19b91-p104">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
