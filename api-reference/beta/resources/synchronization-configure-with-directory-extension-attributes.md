---
title: Configurar a sincronização com atributos de extensão de diretório
description: Personalize seu esquema de sincronização para incluir Azure Active Directory de extensão de diretório (Azure AD).
ms.localizationpriority: medium
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b3379502f1bf5354d4f53e863f4924c5f251bd4a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976809"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a>Configurar a sincronização com atributos de extensão de diretório

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode personalizar seu esquema de sincronização para incluir Azure Active Directory de extensão de diretório (Azure AD). Este artigo descreve como usar um atributo de extensão de diretório (**extension_9d98asdfl15980a_Nickname**) para preencher o valor de User.CommunityNickname no Salesforce. Nesse cenário, você tem o Azure AD Conexão configurar para provisionar vários atributos de extensão de diretório do Windows Server Active Directory local para o Azure AD. 

Este artigo supõe que você já adicionou um aplicativo que oferece suporte à sincronização ao seu locatário por meio do [Portal do Azure,](https://portal.azure.com)que você conhece o nome de exibição do aplicativo e que tem um token de autorização para o Microsoft Graph. Para obter informações sobre como obter o token de autorização, consulte [Obter tokens de acesso para chamar a Microsoft Graph](/graph/auth/).

## <a name="find-the-service-principal-object-by-display-name"></a>Encontre o objeto de entidade de serviço por nome de exibição

O exemplo a seguir mostra como encontrar um objeto de entidade de serviço com o nome de exibição "Área Desatenção do Salesforce".

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

O `{servicePrincipalId}` é `60443998-8cf7-4e61-b05c-a53b658cb5e1` .

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>Listar trabalhos de sincronização no contexto da entidade de serviço 

O exemplo a seguir mostra como obter o `jobId` que você precisa trabalhar. Geralmente, a resposta retorna apenas um trabalho.

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

O `{jobId}` é `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` .

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a>Encontre o nome do atributo de extensão de diretório de que você precisa

Você precisará do nome completo do atributo extension. Se você não sabe o nome completo (que deve ser semelhante ao extension_9d98asdfl15980a_Nickname **),** confira as seguintes informações sobre atributos de extensão de diretório e como inspecioná-los: 

* [Estendendo o esquema de diretório do Azure AD com propriedades personalizadas](/graph/extensibility-overview)
* [Extensões de esquema de diretório | Graph de API](/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a>Obter o esquema de sincronização
O exemplo a seguir mostra como obter o esquema de sincronização.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-synchronizationschema-3-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas em uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a>Adicione uma definição para o atributo de extensão de diretório e um mapeamento entre os atributos

Use um editor de texto simples de sua escolha [(por exemplo, Bloco de notas++](https://notepad-plus-plus.org/) ou [Editor JSON Online](https://www.jsoneditoronline.org/)) para:

1. Adicione uma [definição de atributo](synchronization-attributedefinition.md) para o `extension_9d98asdfl15980a_Nickname` atributo. 

    - Em diretórios, encontre o diretório com o nome "Azure Active Directory", e na matriz do objeto, encontre o chamado **User**.
    - Adicione o novo atributo à lista, especificando o nome e o tipo, conforme mostrado no exemplo a seguir.

2. Adicione um [mapeamento de atributos](synchronization-attributemapping.md) entre extension_9d98asdfl15980a_Nickname e CommunityNickname.

    - Em [synchronizationRules,](synchronization-synchronizationrule.md)localiza a regra que especifica o Azure AD como diretório de origem e Salesforce.com como o diretório de destino ( `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` ).
    - No [objectMappings](synchronization-objectmapping.md) da regra, encontre o mapeamento entre usuários ( `"sourceObjectName": "User",   "targetObjectName": "User"` ).
    - Na matriz [attributeMappings](synchronization-attributemapping.md) do **objectMapping**, adicione uma nova entrada, conforme mostrado no exemplo a seguir.

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

Ao salvar o esquema de sincronização atualizado, certifique-se de incluir todo o esquema, incluindo as partes nãomodificadas. Essa solicitação substituirá o esquema existente pelo que você fornece.

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

Se o esquema tiver sido salvo com êxito, na próxima iteração do trabalho de sincronização, ele começará a processar todas as contas no Azure AD e os novos mapeamentos serão aplicados a todas as contas provisionadas.
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get the synchronization schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
