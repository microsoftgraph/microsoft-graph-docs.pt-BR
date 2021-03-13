---
title: Listar configurações de grupo
description: Recupere uma lista de objetos de configuração de grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6db805374ce4783ff9d339f128efd7bc416ab161
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761308"
---
# <a name="list-group-settings"></a><span data-ttu-id="7d4a3-103">Listar configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="7d4a3-103">List group settings</span></span>

<span data-ttu-id="7d4a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d4a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d4a3-105">Recupere uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-105">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d4a3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7d4a3-106">Permissions</span></span>

<span data-ttu-id="7d4a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d4a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7d4a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d4a3-109">Permission type</span></span>      | <span data-ttu-id="7d4a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d4a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d4a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d4a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d4a3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d4a3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d4a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d4a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d4a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-114">Not supported.</span></span>    |
|<span data-ttu-id="7d4a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d4a3-115">Application</span></span> | <span data-ttu-id="7d4a3-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d4a3-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d4a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d4a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="7d4a3-118">Listar configurações de grupo ou de locatários.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-118">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d4a3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d4a3-119">Optional query parameters</span></span>
<span data-ttu-id="7d4a3-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="7d4a3-121">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d4a3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d4a3-122">Request headers</span></span>
| <span data-ttu-id="7d4a3-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7d4a3-123">Name</span></span> | <span data-ttu-id="7d4a3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d4a3-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="7d4a3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d4a3-125">Authorization</span></span>  | <span data-ttu-id="7d4a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d4a3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d4a3-128">Request body</span></span>
<span data-ttu-id="7d4a3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d4a3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d4a3-130">Response</span></span>

<span data-ttu-id="7d4a3-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-131">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d4a3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d4a3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7d4a3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d4a3-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7d4a3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d4a3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[<span data-ttu-id="7d4a3-135">C#</span><span class="sxs-lookup"><span data-stu-id="7d4a3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d4a3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d4a3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d4a3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d4a3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d4a3-138">Java</span><span class="sxs-lookup"><span data-stu-id="7d4a3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7d4a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d4a3-139">Response</span></span>

<span data-ttu-id="7d4a3-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d4a3-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

