---
title: Listar configurações de grupo
description: Recupere uma lista de objetos de configuração de grupo.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 69d38e88cecfa64b26cf8e8c4ee152be074edfaa
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679768"
---
# <a name="list-group-settings"></a><span data-ttu-id="e639f-103">Listar configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="e639f-103">List group settings</span></span>

<span data-ttu-id="e639f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e639f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e639f-105">Recupere uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="e639f-105">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e639f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e639f-106">Permissions</span></span>

<span data-ttu-id="e639f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e639f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e639f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e639f-109">Permission type</span></span>      | <span data-ttu-id="e639f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e639f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e639f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e639f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e639f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e639f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e639f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e639f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e639f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e639f-114">Not supported.</span></span>    |
|<span data-ttu-id="e639f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e639f-115">Application</span></span> | <span data-ttu-id="e639f-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e639f-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e639f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e639f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="e639f-118">Listar configurações de grupo ou de locatários.</span><span class="sxs-lookup"><span data-stu-id="e639f-118">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e639f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e639f-119">Optional query parameters</span></span>
<span data-ttu-id="e639f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e639f-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="e639f-121">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="e639f-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e639f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e639f-122">Request headers</span></span>
| <span data-ttu-id="e639f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e639f-123">Name</span></span> | <span data-ttu-id="e639f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e639f-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="e639f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e639f-125">Authorization</span></span>  | <span data-ttu-id="e639f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e639f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e639f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e639f-128">Request body</span></span>
<span data-ttu-id="e639f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e639f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e639f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e639f-130">Response</span></span>

<span data-ttu-id="e639f-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e639f-131">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e639f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e639f-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e639f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e639f-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e639f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e639f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[<span data-ttu-id="e639f-135">C#</span><span class="sxs-lookup"><span data-stu-id="e639f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e639f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e639f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e639f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e639f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e639f-138">Java</span><span class="sxs-lookup"><span data-stu-id="e639f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e639f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e639f-139">Response</span></span>

<span data-ttu-id="e639f-140">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e639f-140">Note: The response object shown here might be shortened for readability.</span></span>
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

