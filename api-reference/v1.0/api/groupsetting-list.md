---
title: Configurações de grupo de lista
description: Recupere uma lista de objetos de configuração de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0066cad3a8f8ee88c20542d428bf7d9809f2e14f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726715"
---
# <a name="list-group-settings"></a><span data-ttu-id="0ed3d-103">Configurações de grupo de lista</span><span class="sxs-lookup"><span data-stu-id="0ed3d-103">List group settings</span></span>

<span data-ttu-id="0ed3d-104">Recupere uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ed3d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ed3d-105">Permissions</span></span>

<span data-ttu-id="0ed3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ed3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0ed3d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ed3d-108">Permission type</span></span>      | <span data-ttu-id="0ed3d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ed3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ed3d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ed3d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ed3d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ed3d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ed3d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ed3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ed3d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-113">Not supported.</span></span>    |
|<span data-ttu-id="0ed3d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ed3d-114">Application</span></span> | <span data-ttu-id="0ed3d-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed3d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ed3d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ed3d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="0ed3d-117">Listar configurações de todo o locatário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ed3d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ed3d-118">Optional query parameters</span></span>
<span data-ttu-id="0ed3d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="0ed3d-120">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-120">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ed3d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ed3d-121">Request headers</span></span>
| <span data-ttu-id="0ed3d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0ed3d-122">Name</span></span> | <span data-ttu-id="0ed3d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ed3d-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0ed3d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ed3d-124">Authorization</span></span>  | <span data-ttu-id="0ed3d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ed3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ed3d-127">Request body</span></span>
<span data-ttu-id="0ed3d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ed3d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ed3d-129">Response</span></span>

<span data-ttu-id="0ed3d-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ed3d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ed3d-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ed3d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ed3d-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0ed3d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ed3d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ed3d-134">C#</span><span class="sxs-lookup"><span data-stu-id="0ed3d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ed3d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ed3d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ed3d-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ed3d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ed3d-137">Java</span><span class="sxs-lookup"><span data-stu-id="0ed3d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ed3d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ed3d-138">Response</span></span>

<span data-ttu-id="0ed3d-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ed3d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
