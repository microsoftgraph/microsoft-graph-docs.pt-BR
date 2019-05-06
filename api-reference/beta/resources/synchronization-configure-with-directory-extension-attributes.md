---
title: Configurar a sincronização com atributos de extensão de diretório
description: 'Você pode personalizar o esquema de sincronização para incluir os atributos de extensão de diretório do Azure Active Directory (Azure AD). Este artigo descreve como usar um atributo de extensão de diretório (**extension_9d98asdfl15980a_Nickname**) para popular o valor de User. CommunityNickname no Salesforce. Neste cenário, você tem o Azure AD Connect configurado para provisionar um número de atributos de extensão de diretório do Windows Server Active Directory no local para o Azure AD. '
localization_priority: Normal
ms.openlocfilehash: 439d70ff4e42513b465b80719be34989c97a810d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620908"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="4a08d-105">Configurar a sincronização com atributos de extensão de diretório</span><span class="sxs-lookup"><span data-stu-id="4a08d-105">Configure synchronization with directory extension attributes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a08d-106">Você pode personalizar o esquema de sincronização para incluir os atributos de extensão de diretório do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="4a08d-106">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="4a08d-107">Este artigo descreve como usar um atributo de extensão de diretório (**extension_9d98asdfl15980a_Nickname**) para popular o valor de User. CommunityNickname no Salesforce.</span><span class="sxs-lookup"><span data-stu-id="4a08d-107">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="4a08d-108">Neste cenário, você tem o Azure AD Connect configurado para provisionar um número de atributos de extensão de diretório do Windows Server Active Directory no local para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a08d-108">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="4a08d-109">Este artigo pressupõe que você já tenha adicionado um aplicativo que oferece suporte à sincronização do seu locatário através do [portal do Azure](https://portal.azure.com), que você conhece o nome de exibição do aplicativo e que você tem um token de autorização para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4a08d-109">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="4a08d-110">Para obter informações sobre como obter o token de autorização, confira [obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="4a08d-110">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="4a08d-111">Localizar o objeto de entidade de serviço por nome de exibição</span><span class="sxs-lookup"><span data-stu-id="4a08d-111">Find the service principal object by display name</span></span>

<span data-ttu-id="4a08d-112">O exemplo a seguir mostra como localizar um objeto de entidade de serviço com o nome de exibição "área restrita" da Salesforce.</span><span class="sxs-lookup"><span data-stu-id="4a08d-112">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="4a08d-113">O `{servicePrincipalId}` é `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span><span class="sxs-lookup"><span data-stu-id="4a08d-113">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="4a08d-114">Listar trabalhos de sincronização no contexto da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="4a08d-114">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="4a08d-115">O exemplo a seguir mostra como obter o `jobId` que você precisa para trabalhar.</span><span class="sxs-lookup"><span data-stu-id="4a08d-115">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="4a08d-116">Geralmente, a resposta retorna apenas um trabalho.</span><span class="sxs-lookup"><span data-stu-id="4a08d-116">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="4a08d-117">O `{jobId}` é `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span><span class="sxs-lookup"><span data-stu-id="4a08d-117">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="4a08d-118">Encontre o nome do atributo de extensão de diretório que você precisa</span><span class="sxs-lookup"><span data-stu-id="4a08d-118">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="4a08d-119">Você precisará do nome completo do atributo de extensão.</span><span class="sxs-lookup"><span data-stu-id="4a08d-119">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="4a08d-120">Se você não souber o nome completo (que deve ser semelhante a **extension_9d98asdfl15980a_Nickname**), Confira as seguintes informações sobre atributos de extensão de diretório e como inspecioná-los:</span><span class="sxs-lookup"><span data-stu-id="4a08d-120">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="4a08d-121">Estender o esquema de diretório do Azure AD com propriedades personalizadas</span><span class="sxs-lookup"><span data-stu-id="4a08d-121">Extending the Azure AD directory schema with custom properties</span></span>](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [<span data-ttu-id="4a08d-122">Extensões de esquema de diretório | Conceitos da API do Graph</span><span class="sxs-lookup"><span data-stu-id="4a08d-122">Directory schema extensions | Graph API concepts</span></span>](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="4a08d-123">Obter o esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="4a08d-123">Get the synchronization schema</span></span>
<span data-ttu-id="4a08d-124">O exemplo a seguir mostra como obter o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4a08d-124">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="4a08d-125">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4a08d-125">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a08d-126">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a08d-126">All the properties will be returned in an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4a08d-127">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4a08d-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a08d-128">Basic</span><span class="sxs-lookup"><span data-stu-id="4a08d-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a08d-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a08d-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="4a08d-130">Adicionar uma definição para o atributo de extensão de diretório e um mapeamento entre os atributos</span><span class="sxs-lookup"><span data-stu-id="4a08d-130">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="4a08d-131">Use um editor de texto sem formatação de sua escolha (por exemplo, [bloco de notas + +](https://notepad-plus-plus.org/) ou [Editor JSON online](https://www.jsoneditoronline.org/)) para:</span><span class="sxs-lookup"><span data-stu-id="4a08d-131">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="4a08d-132">Adicione uma [definição de atributo](synchronization-attributedefinition.md) para `extension_9d98asdfl15980a_Nickname` o atributo.</span><span class="sxs-lookup"><span data-stu-id="4a08d-132">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="4a08d-133">Em diretórios, encontre o diretório com o nome "Azure Active Directory" e, na matriz do objeto, localize aquele chamado **usuário**.</span><span class="sxs-lookup"><span data-stu-id="4a08d-133">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="4a08d-134">Adicione o novo atributo à lista, especificando o nome e o tipo, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4a08d-134">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="4a08d-135">Adicione um [mapeamento de atributos](synchronization-attributemapping.md) entre Extension_9d98asdfl15980a_Nickname e CommunityNickname.</span><span class="sxs-lookup"><span data-stu-id="4a08d-135">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="4a08d-136">Em [synchronizationRules](synchronization-synchronizationrule.md), localize a regra que especifica o Azure ad como diretório de origem e Salesforce.com como o diretório de`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`destino ().</span><span class="sxs-lookup"><span data-stu-id="4a08d-136">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="4a08d-137">Nos objectmappings da regra, encontre o mapeamento entre usuários ( [](synchronization-objectmapping.md) `"sourceObjectName": "User",   "targetObjectName": "User"`).</span><span class="sxs-lookup"><span data-stu-id="4a08d-137">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="4a08d-138">Na matriz [attributeMappings](synchronization-attributemapping.md) do objectmapping \*\*\*\*, adicione uma nova entrada, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4a08d-138">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="4a08d-139">Salvar o esquema de sincronização modificado</span><span class="sxs-lookup"><span data-stu-id="4a08d-139">Save the modified synchronization schema</span></span>

<span data-ttu-id="4a08d-140">Ao salvar o esquema de sincronização atualizado, certifique-se de incluir o esquema inteiro, incluindo as partes não modificadas.</span><span class="sxs-lookup"><span data-stu-id="4a08d-140">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="4a08d-141">Essa solicitação substituirá o esquema existente pelo que você fornecer.</span><span class="sxs-lookup"><span data-stu-id="4a08d-141">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="4a08d-142">Se o esquema foi salvo com êxito, na próxima iteração do trabalho de sincronização, ele começará a reprocessar todas as contas em seu Azure AD e os novos mapeamentos serão aplicados a todas as contas provisionadas.</span><span class="sxs-lookup"><span data-stu-id="4a08d-142">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get the synchronization schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
