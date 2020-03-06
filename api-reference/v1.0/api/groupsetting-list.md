---
title: Configurações de grupo de lista
description: Recupere uma lista de objetos de configuração de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e1fbb56a660c2f111d1e16de549430bde31eec6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516826"
---
# <a name="list-group-settings"></a><span data-ttu-id="feb48-103">Configurações de grupo de lista</span><span class="sxs-lookup"><span data-stu-id="feb48-103">List group settings</span></span>

<span data-ttu-id="feb48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feb48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="feb48-105">Recupere uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="feb48-105">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="feb48-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="feb48-106">Permissions</span></span>

<span data-ttu-id="feb48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="feb48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="feb48-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="feb48-109">Permission type</span></span>      | <span data-ttu-id="feb48-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="feb48-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="feb48-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="feb48-111">Delegated (work or school account)</span></span> | <span data-ttu-id="feb48-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="feb48-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="feb48-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="feb48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="feb48-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feb48-114">Not supported.</span></span>    |
|<span data-ttu-id="feb48-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="feb48-115">Application</span></span> | <span data-ttu-id="feb48-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb48-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="feb48-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="feb48-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="feb48-118">Listar configurações de todo o locatário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="feb48-118">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="feb48-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="feb48-119">Optional query parameters</span></span>
<span data-ttu-id="feb48-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="feb48-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="feb48-121">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="feb48-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="feb48-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="feb48-122">Request headers</span></span>
| <span data-ttu-id="feb48-123">Nome</span><span class="sxs-lookup"><span data-stu-id="feb48-123">Name</span></span> | <span data-ttu-id="feb48-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="feb48-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="feb48-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="feb48-125">Authorization</span></span>  | <span data-ttu-id="feb48-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feb48-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="feb48-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="feb48-128">Request body</span></span>
<span data-ttu-id="feb48-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="feb48-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="feb48-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="feb48-130">Response</span></span>

<span data-ttu-id="feb48-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="feb48-131">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="feb48-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="feb48-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="feb48-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="feb48-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="feb48-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="feb48-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[<span data-ttu-id="feb48-135">C#</span><span class="sxs-lookup"><span data-stu-id="feb48-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="feb48-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="feb48-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="feb48-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="feb48-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="feb48-138">Java</span><span class="sxs-lookup"><span data-stu-id="feb48-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="feb48-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="feb48-139">Response</span></span>

<span data-ttu-id="feb48-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="feb48-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
