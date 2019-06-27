---
title: Obter um modelo de configuração de grupo
description: Um modelo de configuração de grupo representa um modelo de configurações das quais as configurações podem ser criadas em um locatário. Essa operação permite a recuperação das propriedades do objeto groupSettingTemplate, incluindo as configurações disponíveis e seus padrões.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b1f90914f7a381e8be2d4bc0dd4e3a5460ce1015
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277123"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="667a3-104">Obter um modelo de configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="667a3-104">Get a group setting template</span></span>

<span data-ttu-id="667a3-p102">Um modelo de configuração de grupo representa um modelo de configurações pelo qual as configurações podem ser criadas dentro de um locatário. Esta operação permite recuperação das propriedades do objeto [groupSettingTemplate](../resources/groupsettingtemplate.md), inclusive as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="667a3-p102">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="667a3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="667a3-107">Permissions</span></span>

<span data-ttu-id="667a3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="667a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="667a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="667a3-110">Permission type</span></span>      | <span data-ttu-id="667a3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="667a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="667a3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="667a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="667a3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="667a3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="667a3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="667a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="667a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="667a3-115">Not supported.</span></span>    |
|<span data-ttu-id="667a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="667a3-116">Application</span></span> | <span data-ttu-id="667a3-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667a3-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="667a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="667a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="667a3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="667a3-119">Optional query parameters</span></span>
<span data-ttu-id="667a3-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="667a3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="667a3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="667a3-121">Request headers</span></span>
| <span data-ttu-id="667a3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="667a3-122">Name</span></span> | <span data-ttu-id="667a3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="667a3-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="667a3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="667a3-124">Authorization</span></span> | <span data-ttu-id="667a3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="667a3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="667a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="667a3-127">Request body</span></span>
<span data-ttu-id="667a3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="667a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="667a3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="667a3-129">Response</span></span>

<span data-ttu-id="667a3-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="667a3-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667a3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="667a3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="667a3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="667a3-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="667a3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="667a3-133">Response</span></span>

<span data-ttu-id="667a3-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="667a3-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="667a3-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="667a3-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="667a3-137">C#</span><span class="sxs-lookup"><span data-stu-id="667a3-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groupsettingtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="667a3-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="667a3-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groupsettingtemplate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="667a3-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="667a3-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_groupsettingtemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/groupsettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
