---
title: Configurar a sincronização com atributos de destino personalizados
description: Você pode personalizar o esquema de sincronização para incluir atributos personalizados que são definidos no diretório de destino. Este artigo descreve como personalizar uma assinatura do Salesforce adicionando um novo campo chamado `officeCode`. Você configura a sincronização do Azure Active Directory (Azure AD) para o Salesforce e para cada usuário, você preencherá o `officeCode` campo na Salesforce com o valor do `extensionAttribute10` campo no Azure AD.
localization_priority: Normal
ms.openlocfilehash: 698c6b1cd05f3146962c9ebd5bd0e52b264a3145
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33621274"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="f8266-105">Configurar a sincronização com atributos de destino personalizados</span><span class="sxs-lookup"><span data-stu-id="f8266-105">Configure synchronization with custom target attributes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8266-106">Você pode personalizar o esquema de sincronização para incluir atributos personalizados que são definidos no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="f8266-106">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="f8266-107">Este artigo descreve como personalizar uma assinatura do Salesforce adicionando um novo campo chamado `officeCode`.</span><span class="sxs-lookup"><span data-stu-id="f8266-107">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="f8266-108">Você configura a sincronização do Azure Active Directory (Azure AD) para o Salesforce e para cada usuário, você preencherá o `officeCode` campo na Salesforce com o valor do `extensionAttribute10` campo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f8266-108">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="f8266-109">Este artigo pressupõe que você já tenha adicionado um aplicativo que oferece suporte à sincronização do seu locatário através do [portal do Azure](https://portal.azure.com), que você conhece o nome de exibição do aplicativo e que você tem um token de autorização para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f8266-109">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="f8266-110">Para obter informações sobre como obter o token de autorização, confira [obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="f8266-110">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="f8266-111">Localizar o objeto de entidade de serviço por nome de exibição</span><span class="sxs-lookup"><span data-stu-id="f8266-111">Find the service principal object by display name</span></span>

<span data-ttu-id="f8266-112">O exemplo a seguir mostra como localizar um objeto de entidade de serviço com o nome de exibição Salesforce.</span><span class="sxs-lookup"><span data-stu-id="f8266-112">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

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

<span data-ttu-id="f8266-113">O `{servicePrincipalId}` é `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span><span class="sxs-lookup"><span data-stu-id="f8266-113">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="f8266-114">Listar trabalhos de sincronização no contexto da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="f8266-114">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="f8266-115">O exemplo a seguir mostra como obter o `jobId` que você precisa para trabalhar.</span><span class="sxs-lookup"><span data-stu-id="f8266-115">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="f8266-116">Geralmente, a resposta retorna apenas um trabalho.</span><span class="sxs-lookup"><span data-stu-id="f8266-116">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="f8266-117">O `{jobId}` é `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span><span class="sxs-lookup"><span data-stu-id="f8266-117">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="f8266-118">Obter o esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="f8266-118">Get the synchronization schema</span></span>
<span data-ttu-id="f8266-119">O exemplo a seguir mostra como obter o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="f8266-119">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="f8266-120">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f8266-120">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f8266-121">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8266-121">All the properties will be returned in an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8266-122">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f8266-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8266-123">Basic</span><span class="sxs-lookup"><span data-stu-id="f8266-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8266-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8266-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="f8266-125">Adicionar uma definição para o atributo officeCode e um mapeamento entre atributos</span><span class="sxs-lookup"><span data-stu-id="f8266-125">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="f8266-126">Use um editor de texto sem formatação de sua escolha (por exemplo, [bloco de notas + +](https://notepad-plus-plus.org/) ou [Editor JSON online](https://www.jsoneditoronline.org/)) para:</span><span class="sxs-lookup"><span data-stu-id="f8266-126">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="f8266-127">Adicione uma [definição de atributo](synchronization-attributedefinition.md) para `officeCode` o atributo.</span><span class="sxs-lookup"><span data-stu-id="f8266-127">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="f8266-128">Em diretórios, encontre o diretório com o nome salesforce.com e, na matriz do objeto, localize aquele chamado **usuário**.</span><span class="sxs-lookup"><span data-stu-id="f8266-128">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="f8266-129">Adicione o novo atributo à lista, especificando o nome e o tipo, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="f8266-129">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="f8266-130">Adicione um [mapeamento](synchronization-attributemapping.md) de atributos `officeCode` entre `extensionAttribute10`o e o.</span><span class="sxs-lookup"><span data-stu-id="f8266-130">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="f8266-131">Em [synchronizationRules](synchronization-synchronizationrule.md), localize a regra que especifica o Azure ad como o diretório de origem e Salesforce.com como o diretório de`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`destino ().</span><span class="sxs-lookup"><span data-stu-id="f8266-131">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="f8266-132">Nos objectmappings da regra, encontre o mapeamento entre usuários ( [](synchronization-objectmapping.md) `"sourceObjectName": "User",   "targetObjectName": "User"`).</span><span class="sxs-lookup"><span data-stu-id="f8266-132">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="f8266-133">Na matriz [attributeMappings](synchronization-attributemapping.md) do objectmapping \*\*\*\*, adicione uma nova entrada, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="f8266-133">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="f8266-134">Salvar o esquema de sincronização modificado</span><span class="sxs-lookup"><span data-stu-id="f8266-134">Save the modified synchronization schema</span></span>

<span data-ttu-id="f8266-135">Ao salvar o esquema de sincronização atualizado, certifique-se de incluir o esquema inteiro, incluindo as partes não modificadas.</span><span class="sxs-lookup"><span data-stu-id="f8266-135">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="f8266-136">Essa solicitação substituirá o esquema existente pelo que você fornecer.</span><span class="sxs-lookup"><span data-stu-id="f8266-136">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="f8266-137">Se o esquema foi salvo com êxito, na próxima iteração do trabalho de sincronização, ele começará a reprocessar todas as contas em seu Azure AD e os novos mapeamentos serão aplicados a todas as contas provisionadas.</span><span class="sxs-lookup"><span data-stu-id="f8266-137">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get the synchronization schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-custom-target-attributes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/resources/synchronization-configure-with-custom-target-attributes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
