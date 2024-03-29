---
title: Atualizar um educationSynchronizationProfile
description: Atualize as propriedades para um perfil de sincronização de dados escolares existente no locatário.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 37c0f882b53a2b545e2c7b16447cc5b23d50efe5
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60068556"
---
# <a name="update-an-educationsynchronizationprofile"></a>Atualizar um educationSynchronizationProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades para um perfil de sincronização de dados escolares [existente](../resources/educationsynchronizationprofile.md) no locatário.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões |
|:-----------|:----------|
| Delegada (conta corporativa ou de estudante) | EduAdministration.ReadWrite |
|Delegada (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /education/synchronizationProfiles
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório.  |
| Content-Type | string | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto synchronizationProfile.](../resources/educationsynchronizationprofile.md)

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `202, Accepted` de resposta e um objeto [synchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "ignored",
  "name": "update_synchronizationProfile"
}-->
```http
PUT https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationcsvdataprovider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ]
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationidentitycreationconfiguration",
        "userDomains": [
            {
                "appliesTo": "student",
                "name": "testschool.edu"
            },
            {
                "appliesTo": "teacher",
                "name": "testschool.edu"
            }
        ]
    },
    "licensesToAssign": [
        {
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "#microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "school": {
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "section": {
                "optionalPropertiesToSync": [
                    "Term Name",
                    "Course Number",
                    "Periods"
                ],
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ],
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacher": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Teacher Number",
                    "Status",
                    "Middle Name",
                    "Secondary Email",
                    "Title",
                    "Qualification"
                ],
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "studentEnrollment": {
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacherRoster": {
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
        "userDomains": [
            {
                "appliesTo": "student",
                "name": "testschool.edu"
            },
            {
                "appliesTo": "teacher",
                "name": "testschool.edu"
            }
        ]
    },
    "licensesToAssign": [
        {
            "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",                
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",                
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```


