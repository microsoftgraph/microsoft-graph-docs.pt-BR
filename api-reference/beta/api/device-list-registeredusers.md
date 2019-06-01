---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 89f6504bc0a6f081c2dff7da193b72cebb783bb8
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656346"
---
# <a name="list-registeredusers"></a><span data-ttu-id="45793-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="45793-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45793-104">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45793-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="45793-105">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="45793-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="45793-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45793-106">Permissions</span></span>
<span data-ttu-id="45793-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45793-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45793-109">Permission type</span></span>      | <span data-ttu-id="45793-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45793-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45793-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45793-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45793-112">Directory. Read. All ou Directory. ReadWrite. All ou Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="45793-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="45793-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45793-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45793-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45793-114">Not supported.</span></span> |
|<span data-ttu-id="45793-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45793-115">Application</span></span> | <span data-ttu-id="45793-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45793-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45793-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45793-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="45793-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="45793-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="45793-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45793-119">Optional query parameters</span></span>
<span data-ttu-id="45793-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45793-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="45793-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45793-121">Request headers</span></span>
| <span data-ttu-id="45793-122">Nome</span><span class="sxs-lookup"><span data-stu-id="45793-122">Name</span></span>       | <span data-ttu-id="45793-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="45793-123">Type</span></span> | <span data-ttu-id="45793-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="45793-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="45793-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="45793-125">Authorization</span></span>  | <span data-ttu-id="45793-126">string</span><span class="sxs-lookup"><span data-stu-id="45793-126">string</span></span>  | <span data-ttu-id="45793-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45793-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45793-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45793-129">Request body</span></span>
<span data-ttu-id="45793-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45793-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45793-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="45793-131">Response</span></span>

<span data-ttu-id="45793-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45793-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45793-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45793-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45793-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45793-134">Request</span></span>
<span data-ttu-id="45793-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45793-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="45793-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="45793-136">Response</span></span>
<span data-ttu-id="45793-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45793-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="45793-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="45793-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="45793-141">C#</span><span class="sxs-lookup"><span data-stu-id="45793-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_registeredusers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45793-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="45793-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_registeredusers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-registeredusers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-list-registeredusers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
