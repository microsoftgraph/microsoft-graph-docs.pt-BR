---
title: Listar grupos transitivos de dispositivo
description: Obter grupos dos quais o dispositivo é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o dispositivo é um membro aninhado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a24094a4a53a51e399de3458f4b3f75db537bc2f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435735"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="833ae-104">Listar grupos transitivos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="833ae-104">List device transitive groups</span></span>

<span data-ttu-id="833ae-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="833ae-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="833ae-106">Obter grupos dos quais o dispositivo é membro.</span><span class="sxs-lookup"><span data-stu-id="833ae-106">Get groups that the device is a member of.</span></span> <span data-ttu-id="833ae-107">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o dispositivo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="833ae-107">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="833ae-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="833ae-108">Permissions</span></span>

<span data-ttu-id="833ae-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="833ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="833ae-111">Permission type</span></span>      | <span data-ttu-id="833ae-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="833ae-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="833ae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="833ae-113">Delegated (work or school account)</span></span> | <span data-ttu-id="833ae-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="833ae-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="833ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="833ae-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="833ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="833ae-116">Not supported.</span></span>    |
|<span data-ttu-id="833ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="833ae-117">Application</span></span> | <span data-ttu-id="833ae-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="833ae-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]


## <a name="http-request"></a><span data-ttu-id="833ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="833ae-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="833ae-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="833ae-120">Optional query parameters</span></span>

<span data-ttu-id="833ae-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="833ae-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="833ae-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="833ae-122">Request headers</span></span>

| <span data-ttu-id="833ae-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="833ae-123">Header</span></span>       | <span data-ttu-id="833ae-124">Valor</span><span class="sxs-lookup"><span data-stu-id="833ae-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="833ae-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="833ae-125">Authorization</span></span>  | <span data-ttu-id="833ae-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="833ae-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="833ae-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="833ae-128">Accept</span></span>  | <span data-ttu-id="833ae-129">application/json</span><span class="sxs-lookup"><span data-stu-id="833ae-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="833ae-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="833ae-130">Request body</span></span>

<span data-ttu-id="833ae-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="833ae-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="833ae-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="833ae-132">Response</span></span>

<span data-ttu-id="833ae-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="833ae-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="833ae-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="833ae-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="833ae-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="833ae-135">Request</span></span>

<span data-ttu-id="833ae-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="833ae-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="833ae-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="833ae-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="833ae-138">C#</span><span class="sxs-lookup"><span data-stu-id="833ae-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="833ae-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="833ae-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="833ae-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="833ae-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="833ae-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="833ae-141">Response</span></span>

<span data-ttu-id="833ae-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="833ae-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
