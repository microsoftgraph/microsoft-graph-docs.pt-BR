---
title: Obter um modelo de configuração de grupo
description: Obtenha um modelo de configuração de grupo que representa um modelo de configurações das quais as configurações podem ser criadas dentro de um locatário.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7af640dcf585499297a4df59ebc7f48b84749728
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402132"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="95fca-103">Obter um modelo de configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="95fca-103">Get a group setting template</span></span>

<span data-ttu-id="95fca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95fca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95fca-p101">Um modelo de configuração de grupo representa um modelo de configurações pelo qual as configurações podem ser criadas dentro de um locatário. Esta operação permite recuperação das propriedades do objeto [groupSettingTemplate](../resources/groupsettingtemplate.md), inclusive as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="95fca-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="95fca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="95fca-107">Permissions</span></span>

<span data-ttu-id="95fca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95fca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="95fca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95fca-110">Permission type</span></span>      | <span data-ttu-id="95fca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95fca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95fca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95fca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="95fca-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95fca-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="95fca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95fca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95fca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95fca-115">Not supported.</span></span>    |
|<span data-ttu-id="95fca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95fca-116">Application</span></span> | <span data-ttu-id="95fca-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95fca-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95fca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95fca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95fca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="95fca-119">Optional query parameters</span></span>
<span data-ttu-id="95fca-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="95fca-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95fca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95fca-121">Request headers</span></span>
| <span data-ttu-id="95fca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="95fca-122">Name</span></span> | <span data-ttu-id="95fca-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="95fca-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="95fca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="95fca-124">Authorization</span></span> | <span data-ttu-id="95fca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95fca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95fca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95fca-127">Request body</span></span>
<span data-ttu-id="95fca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95fca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95fca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="95fca-129">Response</span></span>

<span data-ttu-id="95fca-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95fca-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95fca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95fca-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95fca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95fca-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="95fca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="95fca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="95fca-134">C#</span><span class="sxs-lookup"><span data-stu-id="95fca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95fca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95fca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95fca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95fca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95fca-137">Java</span><span class="sxs-lookup"><span data-stu-id="95fca-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="95fca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="95fca-138">Response</span></span>

<span data-ttu-id="95fca-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95fca-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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