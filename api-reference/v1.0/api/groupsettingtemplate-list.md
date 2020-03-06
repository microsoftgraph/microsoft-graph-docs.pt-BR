---
title: Lista groupSettingTemplates
description: Os Modelos de configuração de grupo representam um conjunto de modelos pelo qual as configurações de grupo podem ser criadas e usadas em um locatário.  Esta operação recupera a lista de objetos groupSettingTemplates disponíveis.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d529d7d012a3bdf15c14fcd01482787ba5656636
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516798"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="233f7-104">Lista groupSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="233f7-104">List groupSettingTemplates</span></span>

<span data-ttu-id="233f7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="233f7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="233f7-p102">Os Modelos de configuração de grupo representam um conjunto de modelos pelo qual as configurações de grupo podem ser criadas e usadas em um locatário.  Esta operação recupera a lista de objetos groupSettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="233f7-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="233f7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="233f7-108">Permissions</span></span>

<span data-ttu-id="233f7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="233f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="233f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="233f7-111">Permission type</span></span>      | <span data-ttu-id="233f7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="233f7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="233f7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="233f7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="233f7-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="233f7-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="233f7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="233f7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="233f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="233f7-116">Not supported.</span></span>    |
|<span data-ttu-id="233f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="233f7-117">Application</span></span> | <span data-ttu-id="233f7-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233f7-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="233f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="233f7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="233f7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="233f7-120">Optional query parameters</span></span>
<span data-ttu-id="233f7-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="233f7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="233f7-122">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="233f7-122">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="233f7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="233f7-123">Request headers</span></span>
| <span data-ttu-id="233f7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="233f7-124">Name</span></span> | <span data-ttu-id="233f7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="233f7-125">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="233f7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="233f7-126">Authorization</span></span>  | <span data-ttu-id="233f7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="233f7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="233f7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="233f7-129">Request body</span></span>
<span data-ttu-id="233f7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="233f7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="233f7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="233f7-131">Response</span></span>

<span data-ttu-id="233f7-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="233f7-132">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="233f7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="233f7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="233f7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="233f7-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="233f7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="233f7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="233f7-136">C#</span><span class="sxs-lookup"><span data-stu-id="233f7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="233f7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="233f7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="233f7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="233f7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="233f7-139">Java</span><span class="sxs-lookup"><span data-stu-id="233f7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="233f7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="233f7-140">Response</span></span>

<span data-ttu-id="233f7-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="233f7-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
                    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
                    "deletedDateTime": null,
                    "displayName": "Group.Unified",
                    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
                    "values": [
                        {
                            "name": "CustomBlockedWordsList",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "EnableMSStandardBlockedWords",
                            "type": "System.Boolean",
                            "defaultValue": "false",
                            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "ClassificationDescriptions",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
                        }
                    ]
                }
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
