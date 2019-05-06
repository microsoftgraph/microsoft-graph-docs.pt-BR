---
title: Listar grupos transitivos de dispositivo
description: Obter grupos dos quais o dispositivo é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o dispositivo é um membro aninhado.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8325219b3256555f7f88216b62fc98c758fb7b79
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590912"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="29a6d-104">Listar grupos transitivos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="29a6d-104">List device transitive groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29a6d-105">Obter grupos dos quais o dispositivo é membro.</span><span class="sxs-lookup"><span data-stu-id="29a6d-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="29a6d-106">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o dispositivo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="29a6d-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="29a6d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="29a6d-107">Permissions</span></span>

<span data-ttu-id="29a6d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29a6d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29a6d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29a6d-110">Permission type</span></span>      | <span data-ttu-id="29a6d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29a6d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29a6d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29a6d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29a6d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29a6d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29a6d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29a6d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29a6d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29a6d-115">Not supported.</span></span>    |
|<span data-ttu-id="29a6d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29a6d-116">Application</span></span> | <span data-ttu-id="29a6d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29a6d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29a6d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29a6d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29a6d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="29a6d-119">Optional query parameters</span></span>

<span data-ttu-id="29a6d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="29a6d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29a6d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29a6d-121">Request headers</span></span>

| <span data-ttu-id="29a6d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29a6d-122">Header</span></span>       | <span data-ttu-id="29a6d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="29a6d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29a6d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="29a6d-124">Authorization</span></span>  | <span data-ttu-id="29a6d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29a6d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29a6d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29a6d-127">Accept</span></span>  | <span data-ttu-id="29a6d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="29a6d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29a6d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29a6d-129">Request body</span></span>

<span data-ttu-id="29a6d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29a6d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29a6d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="29a6d-131">Response</span></span>

<span data-ttu-id="29a6d-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29a6d-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29a6d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29a6d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="29a6d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29a6d-134">Request</span></span>

<span data-ttu-id="29a6d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29a6d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="29a6d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="29a6d-136">Response</span></span>

<span data-ttu-id="29a6d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29a6d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="29a6d-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="29a6d-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="29a6d-141">Basic</span><span class="sxs-lookup"><span data-stu-id="29a6d-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29a6d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29a6d-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
