---
title: Configurar a sincronização com atributos de destino personalizados
description: Você pode personalizar o esquema de sincronização para incluir atributos personalizados que são definidos no diretório de destino. Este artigo descreve como personalizar uma assinatura do Salesforce adicionando um novo campo chamado `officeCode`. Você configura a sincronização do Azure Active Directory (Azure AD) para o Salesforce e para cada usuário, você preencherá o `officeCode` campo na Salesforce com o valor do `extensionAttribute10` campo no Azure AD.
localization_priority: Normal
doc_type: conceptualPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c17f22a1097d99d856ddcbc2611c451f9c5e21a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520223"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="c1a3c-105">Configurar a sincronização com atributos de destino personalizados</span><span class="sxs-lookup"><span data-stu-id="c1a3c-105">Configure synchronization with custom target attributes</span></span>

<span data-ttu-id="c1a3c-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c1a3c-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1a3c-107">Você pode personalizar o esquema de sincronização para incluir atributos personalizados que são definidos no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-107">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="c1a3c-108">Este artigo descreve como personalizar uma assinatura do Salesforce adicionando um novo campo chamado `officeCode`.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-108">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="c1a3c-109">Você configura a sincronização do Azure Active Directory (Azure AD) para o Salesforce e para cada usuário, você preencherá o `officeCode` campo na Salesforce com o valor do `extensionAttribute10` campo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-109">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="c1a3c-110">Este artigo pressupõe que você já tenha adicionado um aplicativo que oferece suporte à sincronização do seu locatário através do [portal do Azure](https://portal.azure.com), que você conhece o nome de exibição do aplicativo e que você tem um token de autorização para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-110">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="c1a3c-111">Para obter informações sobre como obter o token de autorização, confira [obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="c1a3c-111">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="c1a3c-112">Localizar o objeto de entidade de serviço por nome de exibição</span><span class="sxs-lookup"><span data-stu-id="c1a3c-112">Find the service principal object by display name</span></span>

<span data-ttu-id="c1a3c-113">O exemplo a seguir mostra como localizar um objeto de entidade de serviço com o nome de exibição Salesforce.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-113">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

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

<span data-ttu-id="c1a3c-114">O `{servicePrincipalId}` é `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-114">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="c1a3c-115">Listar trabalhos de sincronização no contexto da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="c1a3c-115">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="c1a3c-116">O exemplo a seguir mostra como obter o `jobId` que você precisa para trabalhar.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-116">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="c1a3c-117">Geralmente, a resposta retorna apenas um trabalho.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-117">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="c1a3c-118">O `{jobId}` é `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-118">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="c1a3c-119">Obter o esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="c1a3c-119">Get the synchronization schema</span></span>
<span data-ttu-id="c1a3c-120">O exemplo a seguir mostra como obter o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-120">The following example shows how to get the synchronization schema.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1a3c-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a3c-121">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[<span data-ttu-id="c1a3c-122">C#</span><span class="sxs-lookup"><span data-stu-id="c1a3c-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1a3c-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1a3c-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1a3c-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1a3c-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


><span data-ttu-id="c1a3c-125">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-125">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c1a3c-126">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-126">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="c1a3c-127">Adicionar uma definição para o atributo officeCode e um mapeamento entre atributos</span><span class="sxs-lookup"><span data-stu-id="c1a3c-127">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="c1a3c-128">Use um editor de texto sem formatação de sua escolha (por exemplo, [bloco de notas + +](https://notepad-plus-plus.org/) ou [Editor JSON online](https://www.jsoneditoronline.org/)) para:</span><span class="sxs-lookup"><span data-stu-id="c1a3c-128">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="c1a3c-129">Adicione uma [definição de atributo](synchronization-attributedefinition.md) para `officeCode` o atributo.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-129">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="c1a3c-130">Em diretórios, encontre o diretório com o nome salesforce.com e, na matriz do objeto, localize aquele chamado **usuário**.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-130">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="c1a3c-131">Adicione o novo atributo à lista, especificando o nome e o tipo, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-131">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="c1a3c-132">Adicione um [mapeamento](synchronization-attributemapping.md) de atributos `officeCode` entre `extensionAttribute10`o e o.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-132">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="c1a3c-133">Em [synchronizationRules](synchronization-synchronizationrule.md), localize a regra que especifica o Azure ad como o diretório de origem e Salesforce.com como o diretório de`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`destino ().</span><span class="sxs-lookup"><span data-stu-id="c1a3c-133">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="c1a3c-134">Nos [Objectmappings](synchronization-objectmapping.md) da regra, encontre o mapeamento entre usuários (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span><span class="sxs-lookup"><span data-stu-id="c1a3c-134">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="c1a3c-135">Na matriz [attributeMappings](synchronization-attributemapping.md) do **objectmapping**, adicione uma nova entrada, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-135">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="c1a3c-136">Salvar o esquema de sincronização modificado</span><span class="sxs-lookup"><span data-stu-id="c1a3c-136">Save the modified synchronization schema</span></span>

<span data-ttu-id="c1a3c-137">Ao salvar o esquema de sincronização atualizado, certifique-se de incluir o esquema inteiro, incluindo as partes não modificadas.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-137">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="c1a3c-138">Essa solicitação substituirá o esquema existente pelo que você fornecer.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-138">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="c1a3c-139">Se o esquema foi salvo com êxito, na próxima iteração do trabalho de sincronização, ele começará a reprocessar todas as contas em seu Azure AD e os novos mapeamentos serão aplicados a todas as contas provisionadas.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-139">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
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
