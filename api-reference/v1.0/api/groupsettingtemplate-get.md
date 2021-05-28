---
title: Obter um modelo de configuração de grupo
description: Obter um modelo de configuração de grupo que representa um modelo de configurações a partir dos quais as configurações podem ser criadas em um locatário.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c90fc6b3c30991583765d960173636580c7258e3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679747"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="ee30d-103">Obter um modelo de configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="ee30d-103">Get a group setting template</span></span>

<span data-ttu-id="ee30d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee30d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee30d-p101">Um modelo de configuração de grupo representa um modelo de configurações pelo qual as configurações podem ser criadas dentro de um locatário. Esta operação permite recuperação das propriedades do objeto [groupSettingTemplate](../resources/groupsettingtemplate.md), inclusive as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="ee30d-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee30d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee30d-107">Permissions</span></span>

<span data-ttu-id="ee30d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee30d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ee30d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee30d-110">Permission type</span></span>      | <span data-ttu-id="ee30d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee30d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee30d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee30d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ee30d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee30d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee30d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee30d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee30d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee30d-115">Not supported.</span></span>    |
|<span data-ttu-id="ee30d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee30d-116">Application</span></span> | <span data-ttu-id="ee30d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee30d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee30d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee30d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee30d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee30d-119">Optional query parameters</span></span>
<span data-ttu-id="ee30d-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee30d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee30d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee30d-121">Request headers</span></span>
| <span data-ttu-id="ee30d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ee30d-122">Name</span></span> | <span data-ttu-id="ee30d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee30d-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ee30d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee30d-124">Authorization</span></span> | <span data-ttu-id="ee30d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee30d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee30d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee30d-127">Request body</span></span>
<span data-ttu-id="ee30d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee30d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee30d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee30d-129">Response</span></span>

<span data-ttu-id="ee30d-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee30d-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee30d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee30d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee30d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee30d-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ee30d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee30d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="ee30d-134">C#</span><span class="sxs-lookup"><span data-stu-id="ee30d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee30d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee30d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee30d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee30d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee30d-137">Java</span><span class="sxs-lookup"><span data-stu-id="ee30d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ee30d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee30d-138">Response</span></span>

<span data-ttu-id="ee30d-139">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ee30d-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1341

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates/$entity",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
