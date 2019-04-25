---
title: Configurar a sincronização com atributos de extensão de diretório
description: 'Você pode personalizar o esquema de sincronização para incluir os atributos de extensão de diretório do Azure Active Directory (Azure AD). Este artigo descreve como usar um atributo de extensão de diretório (**extension_9d98asdfl15980a_Nickname**) para popular o valor de User. CommunityNickname no Salesforce. Neste cenário, você tem o Azure AD Connect configurado para provisionar um número de atributos de extensão de diretório do Windows Server Active Directory no local para o Azure AD. '
localization_priority: Normal
ms.openlocfilehash: 4160a95acfc6b23f5d5a9d880f36d9ca6a1f3362
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582112"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a>Configurar a sincronização com atributos de extensão de diretório

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode personalizar o esquema de sincronização para incluir os atributos de extensão de diretório do Azure Active Directory (Azure AD). Este artigo descreve como usar um atributo de extensão de diretório (**extension_9d98asdfl15980a_Nickname**) para popular o valor de User. CommunityNickname no Salesforce. Neste cenário, você tem o Azure AD Connect configurado para provisionar um número de atributos de extensão de diretório do Windows Server Active Directory no local para o Azure AD. 

Este artigo pressupõe que você já tenha adicionado um aplicativo que oferece suporte à sincronização do seu locatário através do [portal do Azure](https://portal.azure.com), que você conhece o nome de exibição do aplicativo e que você tem um token de autorização para o Microsoft Graph. Para obter informações sobre como obter o token de autorização, confira [obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).

## <a name="find-the-service-principal-object-by-display-name"></a>Localizar o objeto de entidade de serviço por nome de exibição

O exemplo a seguir mostra como localizar um objeto de entidade de serviço com o nome de exibição "área restrita" da Salesforce.

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}
```

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals(id,appId,displayName)",
    "value": [
    {
        "id": "167e33e9-f80e-490e-b4d8-698d4a80fb3e",
        "appId": "cd3ed3de-93ee-400b-8b19-b61ef44a0f29",
        "displayName": "Salesforce"
    },
    {
        "id": "8cbbb70b-7290-42da-83ee-89fa3517a977",
        "appId": "b0f2e3b1-fe31-4658-b216-44dcaeabb63a",
        "displayName": "salesforce 1"
    },
    {
        "id": "60443998-8cf7-4e61-b05c-a53b658cb5e1",
        "appId": "79079396-c301-405d-900f-e2e0c2439a90",
        "displayName": "Salesforce Sandbox"
    }
    ]
}
```

O `{servicePrincipalId}` é `60443998-8cf7-4e61-b05c-a53b658cb5e1`.

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>Listar trabalhos de sincronização no contexto da entidade de serviço 

O exemplo a seguir mostra como obter o `jobId` que você precisa para trabalhar. Geralmente, a resposta retorna apenas um trabalho.

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}
```

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('60443998-8cf7-4e61-b05c-a53b658cb5e1')/synchronization/jobs",
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {},
            "status": {}
    }
    ]
}
```

O `{jobId}` é `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a>Encontre o nome do atributo de extensão de diretório que você precisa

Você precisará do nome completo do atributo de extensão. Se você não souber o nome completo (que deve ser semelhante a **extension_9d98asdfl15980a_Nickname**), Confira as seguintes informações sobre atributos de extensão de diretório e como inspecioná-los: 

* [Estender o esquema de diretório do Azure AD com propriedades personalizadas](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [Extensões de esquema de diretório | Conceitos da API do Graph](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a>Obter o esquema de sincronização
O exemplo a seguir mostra como obter o esquema de sincronização.

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas em uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

{
  "directories": [
        {
              "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
              "name": "Azure Active Directory",
              "objects": [
                {
                    "attributes": [
                        {
                          "anchor": true,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "objectId",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        },
                        {
                          "anchor": false,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "streetAddress",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        }
                    ],
                    "name": "User"
                }
             ]
        },
        {
              "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
              "name": "salesforce.com",
              "objects": []
        }
  ],
 "synchronizationRules": [
        {
          "editable": true,
          "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
          "name": "USER_OUTBOUND_USER",
          "objectMappings": [
                {
                    "attributeMappings": [
                            {
                              "defaultValue": "True",
                              "exportMissingReferences": false,
                              "flowBehavior": "FlowWhenChanged",
                              "flowType": "Always",
                              "matchingPriority": 0,
                              "source": {
                                "expression": "Not([IsSoftDeleted])",
                                "name": "Not",
                                "parameters": [
                                  {
                                    "key": "source",
                                    "value": {
                                      "expression": "[IsSoftDeleted]",
                                      "name": "IsSoftDeleted",
                                      "parameters": [],
                                      "type": "Attribute"
                                    }
                                  }
                                ],
                                "type": "Function"
                              },
                              "targetAttributeName": "IsActive"
                            }
                     ],
                    "enabled": true,
                    "flowTypes": "Add, Update, Delete",
                    "name": "Synchronize Azure Active Directory Users to salesforce.com",
                    "scope": null,
                    "sourceObjectName": "User",
                    "targetObjectName": "User"
            }]
        }]
}
```

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a>Adicionar uma definição para o atributo de extensão de diretório e um mapeamento entre os atributos

Use um editor de texto sem formatação de sua escolha (por exemplo, [bloco de notas + +](https://notepad-plus-plus.org/) ou [Editor JSON online](https://www.jsoneditoronline.org/)) para:

1. Adicione uma [definição de atributo](synchronization-attributedefinition.md) para `extension_9d98asdfl15980a_Nickname` o atributo. 

    - Em diretórios, encontre o diretório com o nome "Azure Active Directory" e, na matriz do objeto, localize aquele chamado **usuário**.
    - Adicione o novo atributo à lista, especificando o nome e o tipo, conforme mostrado no exemplo a seguir.

2. Adicione um [mapeamento de atributos](synchronization-attributemapping.md) entre Extension_9d98asdfl15980a_Nickname e CommunityNickname.

    - Em [synchronizationRules](synchronization-synchronizationrule.md), localize a regra que especifica o Azure ad como diretório de origem e Salesforce.com como o diretório de`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`destino ().
    - Nos objectMappings da regra, encontre o mapeamento entre usuários ( [](synchronization-objectmapping.md) `"sourceObjectName": "User",   "targetObjectName": "User"`).
    - Na matriz [attributeMappings](synchronization-attributemapping.md) do objectmapping ****, adicione uma nova entrada, conforme mostrado no exemplo a seguir.

    ```json
    {
        "directories": [
            {
                "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
                "name": "Azure Active Directory",
                "objects": [
                    {
                        "attributes": [
                                ,{
                                "name": "extension_9d98asdfl15980a_Nickname",
                                "type": "String"
                                }
                        ],
                        "name":"User"
                    }]
            }
        ],
        "synchronizationRules": [
            {
            "editable": true,
            "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
            "metadata": [..],
            "name": "USER_OUTBOUND_USER",
            "objectMappings": [
                {
                    "attributeMappings": [
                    ,{
                        "source": {
                            "name": "extension_9d98asdfl15980a_Nickname",
                            "type": "Attribute"
                        },
                        "targetAttributeName": "CommunityNickname"
                        }
                ],
                "name": "Synchronize Azure Active Directory Users to salesforce.com",
                    "scope": null,
                    "sourceObjectName": "User",
                    "targetObjectName": "User"
                }
            ],
            "priority": 1,
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "salesforce.com"
            },
        ]
    }
    ```

## <a name="save-the-modified-synchronization-schema"></a>Salvar o esquema de sincronização modificado

Ao salvar o esquema de sincronização atualizado, certifique-se de incluir o esquema inteiro, incluindo as partes não modificadas. Essa solicitação substituirá o esquema existente pelo que você fornecer.

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

Se o esquema foi salvo com êxito, na próxima iteração do trabalho de sincronização, ele começará a reprocessar todas as contas em seu Azure AD e os novos mapeamentos serão aplicados a todas as contas provisionadas.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
