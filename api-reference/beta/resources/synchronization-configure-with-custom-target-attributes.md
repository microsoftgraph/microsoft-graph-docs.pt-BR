---
title: Configurar a sincronização com atributos personalizados de destino
description: Você pode personalizar seu esquema de sincronização para incluir atributos personalizados que são definidos no diretório de destino. Este artigo descreve como personalizar uma assinatura de equipe de vendas, adicionando um novo campo denominado `officeCode`. Configurar a sincronização do Azure Active Directory (AD Azure) para a equipe de vendas e para cada usuário, você preencherá o `officeCode` campo na equipe de vendas com o valor do `extensionAttribute10` campo no Azure AD.
localization_priority: Normal
ms.openlocfilehash: 3a7612682794109a5f94318304c8a8898764ccb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806752"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a>Configurar a sincronização com atributos personalizados de destino

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode personalizar seu esquema de sincronização para incluir atributos personalizados que são definidos no diretório de destino. Este artigo descreve como personalizar uma assinatura de equipe de vendas, adicionando um novo campo denominado `officeCode`. Configurar a sincronização do Azure Active Directory (AD Azure) para a equipe de vendas e para cada usuário, você preencherá o `officeCode` campo na equipe de vendas com o valor do `extensionAttribute10` campo no Azure AD.

Este artigo pressupõe que você já tenha adicionado a um aplicativo que oferece suporte à sincronização ao seu locatário através do [Portal do Windows Azure](https://portal.azure.com), você sabe o nome de exibição do aplicativo, e você tem um token de autorização para o Microsoft Graph. Para obter informações sobre como obter o token de autorização, consulte [tokens de acesso de Get para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).

## <a name="find-the-service-principal-object-by-display-name"></a>Localizar o objeto de entidade de serviço por nome para exibição

O exemplo a seguir mostra como localizar um objeto de entidade de serviço com o nome de exibição a equipe de vendas.

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}

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

O `{servicePrincipalId}` é `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>Trabalhos de sincronização de lista no contexto da entidade de serviço 

O exemplo a seguir mostra como obter o `jobId` que você precisa para trabalhar com. Geralmente, a resposta retorna somente um trabalho.

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}

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

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Serão retornadas todas as propriedades em uma chamada real.

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a>Adicione uma definição para o atributo officeCode e um mapeamento entre os atributos

Use um editor de texto sem formatação de sua preferência (por exemplo, [o bloco de notas + +](https://notepad-plus-plus.org/) ou [Editor JSON Online](https://www.jsoneditoronline.org/)) para:

1. Adicionar uma [definição de atributo](synchronization-attributedefinition.md) para o `officeCode` atributo. 

    - Em diretórios, encontre o diretório com o nome salesforce.com e na matriz do objeto, encontre o nomeado de um **usuário**.
    - Adicione o novo atributo à lista, especificando o nome e tipo, conforme mostrado no exemplo a seguir.

2. Adicionar um [mapeamento de atributo](synchronization-attributemapping.md) entre `officeCode` e `extensionAttribute10`.

    - Em [synchronizationRules](synchronization-synchronizationrule.md), localize a regra que especifica o Azure AD como o diretório de origem e Salesforce.com como o diretório de destino (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).
    - Em [objectMappings](synchronization-objectmapping.md) da regra, localize o mapeamento entre usuários (`"sourceObjectName": "User",   "targetObjectName": "User"`).
    - Na matriz [attributeMappings](synchronization-attributemapping.md) do **objectMapping**, adicione uma nova entrada, conforme mostrado no exemplo a seguir.

```json
{  
    "directories": [
    {
        "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
            "name": "salesforce.com",
            "objects": [
            {
                "attributes": [
                        {
                            "name": "officeCode",
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
        "name": "USER_OUTBOUND_USER",
        "objectMappings": [
            {
            "attributeMappings": [
                {
                    "source": {
                            "name": "extensionAttribute10",
                            "type": "Attribute"
                        },
                    "targetAttributeName": "officeCode"
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
    }
    ]
}
```

## <a name="save-the-modified-synchronization-schema"></a>Salvar o esquema de sincronização modificadas

Quando você salva o esquema de sincronização atualizados, certifique-se de que você inclua o esquema inteiro, incluindo as partes não modificadas. Essa solicitação substituirão o esquema existente com aquele que você fornecer.

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

Se o esquema foi salvo com êxito, na iteração seguinte do trabalho de sincronização, ele iniciará o processamento novamente todas as contas no seu Azure AD e os novos mapeamentos serão aplicados a todas as contas provisionadas.
