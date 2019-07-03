---
title: Listar grupos transitivos de dispositivo
description: Obter grupos dos quais o dispositivo é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o dispositivo é um membro aninhado.
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f73efd6d096a860f51a4d86190e25bf7f26d8135
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461257"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="5ce7e-104">Listar grupos transitivos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5ce7e-104">List device transitive groups</span></span>

<span data-ttu-id="5ce7e-105">Obter grupos dos quais o dispositivo é membro.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="5ce7e-106">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o dispositivo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ce7e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ce7e-107">Permissions</span></span>

<span data-ttu-id="5ce7e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ce7e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ce7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ce7e-110">Permission type</span></span>      | <span data-ttu-id="5ce7e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ce7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ce7e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ce7e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ce7e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ce7e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ce7e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ce7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ce7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-115">Not supported.</span></span>    |
|<span data-ttu-id="5ce7e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ce7e-116">Application</span></span> | <span data-ttu-id="5ce7e-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ce7e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ce7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ce7e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ce7e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ce7e-119">Optional query parameters</span></span>

<span data-ttu-id="5ce7e-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ce7e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce7e-121">Request headers</span></span>

| <span data-ttu-id="5ce7e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ce7e-122">Header</span></span>       | <span data-ttu-id="5ce7e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5ce7e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ce7e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ce7e-124">Authorization</span></span>  | <span data-ttu-id="5ce7e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5ce7e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ce7e-127">Accept</span></span>  | <span data-ttu-id="5ce7e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5ce7e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ce7e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce7e-129">Request body</span></span>

<span data-ttu-id="5ce7e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ce7e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ce7e-131">Response</span></span>

<span data-ttu-id="5ce7e-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ce7e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ce7e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ce7e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ce7e-134">Request</span></span>

<span data-ttu-id="5ce7e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5ce7e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ce7e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ce7e-137">C#</span><span class="sxs-lookup"><span data-stu-id="5ce7e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ce7e-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="5ce7e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ce7e-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5ce7e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ce7e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ce7e-140">Response</span></span>

<span data-ttu-id="5ce7e-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-141">Here is an example of the response.</span></span> 

><span data-ttu-id="5ce7e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ce7e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
