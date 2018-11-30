---
title: Configurar a sincronização com atributos personalizados de destino
description: Você pode personalizar seu esquema de sincronização para incluir atributos personalizados que são definidos no diretório de destino. Este artigo descreve como personalizar uma assinatura de equipe de vendas, adicionando um novo campo denominado `officeCode`. Configurar a sincronização do Azure Active Directory (AD Azure) para a equipe de vendas e para cada usuário, você preencherá o `officeCode` campo na equipe de vendas com o valor do `extensionAttribute10` campo no Azure AD.
ms.openlocfilehash: e043fa5e458a56312871567bb14598f9232e97eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036304"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="4c65e-105">Configurar a sincronização com atributos personalizados de destino</span><span class="sxs-lookup"><span data-stu-id="4c65e-105">Configure synchronization with custom target attributes</span></span>

> <span data-ttu-id="4c65e-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4c65e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c65e-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4c65e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c65e-108">Você pode personalizar seu esquema de sincronização para incluir atributos personalizados que são definidos no diretório de destino.</span><span class="sxs-lookup"><span data-stu-id="4c65e-108">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="4c65e-109">Este artigo descreve como personalizar uma assinatura de equipe de vendas, adicionando um novo campo denominado `officeCode`.</span><span class="sxs-lookup"><span data-stu-id="4c65e-109">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="4c65e-110">Configurar a sincronização do Azure Active Directory (AD Azure) para a equipe de vendas e para cada usuário, você preencherá o `officeCode` campo na equipe de vendas com o valor do `extensionAttribute10` campo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c65e-110">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="4c65e-111">Este artigo pressupõe que você já tenha adicionado a um aplicativo que oferece suporte à sincronização ao seu locatário através do [Portal do Windows Azure](https://portal.azure.com), você sabe o nome de exibição do aplicativo, e você tem um token de autorização para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4c65e-111">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="4c65e-112">Para obter informações sobre como obter o token de autorização, consulte [tokens de acesso de Get para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="4c65e-112">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="4c65e-113">Localizar o objeto de entidade de serviço por nome para exibição</span><span class="sxs-lookup"><span data-stu-id="4c65e-113">Find the service principal object by display name</span></span>

<span data-ttu-id="4c65e-114">O exemplo a seguir mostra como localizar um objeto de entidade de serviço com o nome de exibição a equipe de vendas.</span><span class="sxs-lookup"><span data-stu-id="4c65e-114">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

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

<span data-ttu-id="4c65e-115">O `{servicePrincipalId}` é `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span><span class="sxs-lookup"><span data-stu-id="4c65e-115">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="4c65e-116">Trabalhos de sincronização de lista no contexto da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="4c65e-116">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="4c65e-117">O exemplo a seguir mostra como obter o `jobId` que você precisa para trabalhar com.</span><span class="sxs-lookup"><span data-stu-id="4c65e-117">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="4c65e-118">Geralmente, a resposta retorna somente um trabalho.</span><span class="sxs-lookup"><span data-stu-id="4c65e-118">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="4c65e-119">O `{jobId}` é `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span><span class="sxs-lookup"><span data-stu-id="4c65e-119">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="4c65e-120">Obter o esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="4c65e-120">Get the synchronization schema</span></span>
<span data-ttu-id="4c65e-121">O exemplo a seguir mostra como obter o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4c65e-121">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="4c65e-122">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4c65e-122">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4c65e-123">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c65e-123">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="4c65e-124">Adicione uma definição para o atributo officeCode e um mapeamento entre os atributos</span><span class="sxs-lookup"><span data-stu-id="4c65e-124">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="4c65e-125">Use um editor de texto sem formatação de sua preferência (por exemplo, [o bloco de notas + +](https://notepad-plus-plus.org/) ou [Editor JSON Online](https://www.jsoneditoronline.org/)) para:</span><span class="sxs-lookup"><span data-stu-id="4c65e-125">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="4c65e-126">Adicionar uma [definição de atributo](synchronization-attributedefinition.md) para o `officeCode` atributo.</span><span class="sxs-lookup"><span data-stu-id="4c65e-126">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="4c65e-127">Em diretórios, encontre o diretório com o nome salesforce.com e na matriz do objeto, encontre o nomeado de um **usuário**.</span><span class="sxs-lookup"><span data-stu-id="4c65e-127">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="4c65e-128">Adicione o novo atributo à lista, especificando o nome e tipo, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4c65e-128">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="4c65e-129">Adicionar um [mapeamento de atributo](synchronization-attributemapping.md) entre `officeCode` e `extensionAttribute10`.</span><span class="sxs-lookup"><span data-stu-id="4c65e-129">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="4c65e-130">Em [synchronizationRules](synchronization-synchronizationrule.md), localize a regra que especifica o Azure AD como o diretório de origem e Salesforce.com como o diretório de destino (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span><span class="sxs-lookup"><span data-stu-id="4c65e-130">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="4c65e-131">Em [objectMappings](synchronization-objectmapping.md) da regra, localize o mapeamento entre usuários (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span><span class="sxs-lookup"><span data-stu-id="4c65e-131">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="4c65e-132">Na matriz [attributeMappings](synchronization-attributemapping.md) do **objectMapping**, adicione uma nova entrada, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4c65e-132">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="4c65e-133">Salvar o esquema de sincronização modificadas</span><span class="sxs-lookup"><span data-stu-id="4c65e-133">Save the modified synchronization schema</span></span>

<span data-ttu-id="4c65e-134">Quando você salva o esquema de sincronização atualizados, certifique-se de que você inclua o esquema inteiro, incluindo as partes não modificadas.</span><span class="sxs-lookup"><span data-stu-id="4c65e-134">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="4c65e-135">Essa solicitação substituirão o esquema existente com aquele que você fornecer.</span><span class="sxs-lookup"><span data-stu-id="4c65e-135">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="4c65e-136">Se o esquema foi salvo com êxito, na iteração seguinte do trabalho de sincronização, ele iniciará o processamento novamente todas as contas no seu Azure AD e os novos mapeamentos serão aplicados a todas as contas provisionadas.</span><span class="sxs-lookup"><span data-stu-id="4c65e-136">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
