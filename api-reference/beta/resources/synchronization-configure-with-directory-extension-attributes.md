---
title: Configurar a sincronização com atributos de extensão de diretório
description: Personalize seu esquema de sincronização para incluir atributos de extensão de diretório do Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1a19db23c5797812c41b10ca281efde887da90fc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131493"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="3e1e3-103">Configurar a sincronização com atributos de extensão de diretório</span><span class="sxs-lookup"><span data-stu-id="3e1e3-103">Configure synchronization with directory extension attributes</span></span>

<span data-ttu-id="3e1e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e1e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e1e3-105">Você pode personalizar seu esquema de sincronização para incluir atributos de extensão de diretório do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="3e1e3-105">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="3e1e3-106">Este artigo descreve como usar um atributo de extensão de diretório (**extension_9d98asdfl15980a_Nickname**) para preencher o valor de User.CommunityNickname no Salesforce.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-106">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="3e1e3-107">Neste cenário, você tem o Azure AD Connect definido para provisionar vários atributos de extensão de diretório do Windows Server Active Directory local para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-107">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="3e1e3-108">Este artigo presume que você já adicionou um aplicativo que dá suporte à sincronização com seu locatário por meio do Portal do [Azure,](https://portal.azure.com)que você sabe o nome de exibição do aplicativo e que tem um token de autorização para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-108">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="3e1e3-109">Para obter informações sobre como obter o token de autorização, confira [Obter tokens de acesso para chamar o Microsoft Graph.](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="3e1e3-109">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="3e1e3-110">Encontrar o objeto de entidade de serviço por nome de exibição</span><span class="sxs-lookup"><span data-stu-id="3e1e3-110">Find the service principal object by display name</span></span>

<span data-ttu-id="3e1e3-111">O exemplo a seguir mostra como encontrar um objeto de entidade de serviço com o nome de exibição "Salesforce Sandbox".</span><span class="sxs-lookup"><span data-stu-id="3e1e3-111">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="3e1e3-112">O `{servicePrincipalId}` é `60443998-8cf7-4e61-b05c-a53b658cb5e1` .</span><span class="sxs-lookup"><span data-stu-id="3e1e3-112">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="3e1e3-113">Listar trabalhos de sincronização no contexto da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="3e1e3-113">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="3e1e3-114">O exemplo a seguir mostra como obter `jobId` o que você precisa para trabalhar.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-114">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="3e1e3-115">Geralmente, a resposta retorna apenas um trabalho.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-115">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="3e1e3-116">O `{jobId}` é `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` .</span><span class="sxs-lookup"><span data-stu-id="3e1e3-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="3e1e3-117">Encontre o nome do atributo de extensão de diretório de que você precisa</span><span class="sxs-lookup"><span data-stu-id="3e1e3-117">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="3e1e3-118">Você precisará do nome completo do atributo de extensão.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-118">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="3e1e3-119">Se você não sabe o nome completo (que deve ser semelhante ao **extension_9d98asdfl15980a_Nickname**), consulte as seguintes informações sobre atributos de extensão de diretório e como inspecioná-los:</span><span class="sxs-lookup"><span data-stu-id="3e1e3-119">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="3e1e3-120">Estendendo o esquema de diretório do Azure AD com propriedades personalizadas</span><span class="sxs-lookup"><span data-stu-id="3e1e3-120">Extending the Azure AD directory schema with custom properties</span></span>](/graph/extensibility-overview)
* [<span data-ttu-id="3e1e3-121">Extensões de esquema de | Conceitos da API do Graph</span><span class="sxs-lookup"><span data-stu-id="3e1e3-121">Directory schema extensions | Graph API concepts</span></span>](/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="3e1e3-122">Obter o esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="3e1e3-122">Get the synchronization schema</span></span>
<span data-ttu-id="3e1e3-123">O exemplo a seguir mostra como obter o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-123">The following example shows how to get the synchronization schema.</span></span>


# <a name="http"></a>[<span data-ttu-id="3e1e3-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e1e3-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[<span data-ttu-id="3e1e3-125">C#</span><span class="sxs-lookup"><span data-stu-id="3e1e3-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e1e3-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e1e3-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e1e3-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e1e3-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e1e3-128">Java</span><span class="sxs-lookup"><span data-stu-id="3e1e3-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


><span data-ttu-id="3e1e3-129">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-129">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3e1e3-130">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-130">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="3e1e3-131">Adicionar uma definição para o atributo de extensão de diretório e um mapeamento entre os atributos</span><span class="sxs-lookup"><span data-stu-id="3e1e3-131">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="3e1e3-132">Use um editor de texto sem texto de sua preferência (por exemplo, Bloco de [Notas++](https://notepad-plus-plus.org/) ou [Editor JSON Online](https://www.jsoneditoronline.org/)) para:</span><span class="sxs-lookup"><span data-stu-id="3e1e3-132">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="3e1e3-133">Adicione uma [definição de](synchronization-attributedefinition.md) atributo para o `extension_9d98asdfl15980a_Nickname` atributo.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-133">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="3e1e3-134">Em diretórios, encontre o diretório com o nome "Azure Active Directory" e, na matriz do objeto, encontre o chamado **Usuário**.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-134">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="3e1e3-135">Adicione o novo atributo à lista, especificando o nome e o tipo, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-135">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="3e1e3-136">Adicione um [mapeamento de atributos](synchronization-attributemapping.md) entre extension_9d98asdfl15980a_Nickname e CommunityNickname.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-136">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="3e1e3-137">Em [synchronizationRules](synchronization-synchronizationrule.md), encontre a regra que especifica o Azure AD como diretório de origem e Salesforce.com como o diretório de destino ( `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` ).</span><span class="sxs-lookup"><span data-stu-id="3e1e3-137">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="3e1e3-138">Nos [objectMappings](synchronization-objectmapping.md) da regra, encontre o mapeamento entre os usuários ( `"sourceObjectName": "User",   "targetObjectName": "User"` ).</span><span class="sxs-lookup"><span data-stu-id="3e1e3-138">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="3e1e3-139">Na matriz [attributeMappings](synchronization-attributemapping.md) do **objectMapping,** adicione uma nova entrada, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-139">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="3e1e3-140">Salvar o esquema de sincronização modificado</span><span class="sxs-lookup"><span data-stu-id="3e1e3-140">Save the modified synchronization schema</span></span>

<span data-ttu-id="3e1e3-141">Ao salvar o esquema de sincronização atualizado, certifique-se de incluir todo o esquema, incluindo as partes não modificadas.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-141">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="3e1e3-142">Essa solicitação substituirá o esquema existente pelo que você fornecer.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-142">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="3e1e3-143">Se o esquema foi salvo com êxito, na próxima iteração do trabalho de sincronização, ele começará a processar todas as contas no Azure AD e os novos mapeamentos serão aplicados a todas as contas provisionadas.</span><span class="sxs-lookup"><span data-stu-id="3e1e3-143">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
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
