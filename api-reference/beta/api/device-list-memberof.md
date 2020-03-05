---
title: Listar grupos de dispositivos
description: Obter grupos dos quais este dispositivo é membro direto. Essa operação não é transitiva.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d6020ea3a0be67b55e573b71c93235a5896c5e5b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435854"
---
# <a name="list-device-groups"></a><span data-ttu-id="a55ab-104">Listar grupos de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a55ab-104">List device groups</span></span>

<span data-ttu-id="a55ab-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a55ab-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a55ab-106">Obter grupos dos quais este dispositivo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="a55ab-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="a55ab-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a55ab-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a55ab-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a55ab-108">Permissions</span></span>

<span data-ttu-id="a55ab-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a55ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a55ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a55ab-111">Permission type</span></span>      | <span data-ttu-id="a55ab-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a55ab-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a55ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a55ab-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a55ab-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a55ab-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a55ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a55ab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a55ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a55ab-116">Not supported.</span></span>    |
|<span data-ttu-id="a55ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a55ab-117">Application</span></span> | <span data-ttu-id="a55ab-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a55ab-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a55ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a55ab-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a55ab-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a55ab-120">Optional query parameters</span></span>
<span data-ttu-id="a55ab-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a55ab-121">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a55ab-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a55ab-122">Request headers</span></span>
| <span data-ttu-id="a55ab-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a55ab-123">Header</span></span>       | <span data-ttu-id="a55ab-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a55ab-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a55ab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a55ab-125">Authorization</span></span>  | <span data-ttu-id="a55ab-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a55ab-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a55ab-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a55ab-128">Accept</span></span>  | <span data-ttu-id="a55ab-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a55ab-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a55ab-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a55ab-130">Request body</span></span>
<span data-ttu-id="a55ab-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a55ab-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a55ab-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55ab-132">Response</span></span>

<span data-ttu-id="a55ab-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a55ab-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a55ab-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a55ab-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="a55ab-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a55ab-135">Request</span></span>

<span data-ttu-id="a55ab-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a55ab-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a55ab-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a55ab-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="a55ab-138">C#</span><span class="sxs-lookup"><span data-stu-id="a55ab-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a55ab-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a55ab-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a55ab-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a55ab-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a55ab-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55ab-141">Response</span></span>
<span data-ttu-id="a55ab-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a55ab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
