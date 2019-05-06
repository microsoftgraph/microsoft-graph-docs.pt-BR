---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 857e41899c36cf7dc9600fa788e400770333d6ec
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590891"
---
# <a name="list-registeredusers"></a><span data-ttu-id="228e4-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="228e4-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="228e4-104">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="228e4-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="228e4-105">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="228e4-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="228e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="228e4-106">Permissions</span></span>
<span data-ttu-id="228e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="228e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="228e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="228e4-109">Permission type</span></span>      | <span data-ttu-id="228e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="228e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="228e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="228e4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="228e4-112">Directory. Read. All ou Directory. ReadWrite. All ou Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="228e4-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="228e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="228e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="228e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="228e4-114">Not supported.</span></span> |
|<span data-ttu-id="228e4-115">Application</span><span class="sxs-lookup"><span data-stu-id="228e4-115">Application</span></span> | <span data-ttu-id="228e4-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228e4-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="228e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="228e4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="228e4-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="228e4-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="228e4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="228e4-119">Optional query parameters</span></span>
<span data-ttu-id="228e4-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="228e4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="228e4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="228e4-121">Request headers</span></span>
| <span data-ttu-id="228e4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="228e4-122">Name</span></span>       | <span data-ttu-id="228e4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="228e4-123">Type</span></span> | <span data-ttu-id="228e4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="228e4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="228e4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="228e4-125">Authorization</span></span>  | <span data-ttu-id="228e4-126">string</span><span class="sxs-lookup"><span data-stu-id="228e4-126">string</span></span>  | <span data-ttu-id="228e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="228e4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="228e4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="228e4-129">Request body</span></span>
<span data-ttu-id="228e4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="228e4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="228e4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="228e4-131">Response</span></span>

<span data-ttu-id="228e4-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="228e4-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="228e4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="228e4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="228e4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="228e4-134">Request</span></span>
<span data-ttu-id="228e4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="228e4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="228e4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="228e4-136">Response</span></span>
<span data-ttu-id="228e4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="228e4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="228e4-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="228e4-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="228e4-141">Basic</span><span class="sxs-lookup"><span data-stu-id="228e4-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_registeredusers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="228e4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="228e4-142">Javascript</span></span>](#tab/javascript)
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
