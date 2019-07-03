---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bb9ab8f0176dc825222bd97d92f9fe69b356a494
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437247"
---
# <a name="list-registeredusers"></a><span data-ttu-id="01eb5-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="01eb5-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01eb5-104">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01eb5-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="01eb5-105">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="01eb5-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="01eb5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="01eb5-106">Permissions</span></span>
<span data-ttu-id="01eb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01eb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01eb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01eb5-109">Permission type</span></span>      | <span data-ttu-id="01eb5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01eb5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01eb5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01eb5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01eb5-112">Directory. Read. All ou Directory. ReadWrite. All ou Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="01eb5-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01eb5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01eb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01eb5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01eb5-114">Not supported.</span></span> |
|<span data-ttu-id="01eb5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01eb5-115">Application</span></span> | <span data-ttu-id="01eb5-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01eb5-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01eb5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01eb5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="01eb5-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="01eb5-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="01eb5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01eb5-119">Optional query parameters</span></span>
<span data-ttu-id="01eb5-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="01eb5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="01eb5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01eb5-121">Request headers</span></span>
| <span data-ttu-id="01eb5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="01eb5-122">Name</span></span>       | <span data-ttu-id="01eb5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="01eb5-123">Type</span></span> | <span data-ttu-id="01eb5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="01eb5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01eb5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="01eb5-125">Authorization</span></span>  | <span data-ttu-id="01eb5-126">string</span><span class="sxs-lookup"><span data-stu-id="01eb5-126">string</span></span>  | <span data-ttu-id="01eb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01eb5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01eb5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01eb5-129">Request body</span></span>
<span data-ttu-id="01eb5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01eb5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01eb5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="01eb5-131">Response</span></span>

<span data-ttu-id="01eb5-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01eb5-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01eb5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01eb5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01eb5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01eb5-134">Request</span></span>
<span data-ttu-id="01eb5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01eb5-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01eb5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="01eb5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="01eb5-137">C#</span><span class="sxs-lookup"><span data-stu-id="01eb5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01eb5-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="01eb5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01eb5-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="01eb5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01eb5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="01eb5-140">Response</span></span>
<span data-ttu-id="01eb5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01eb5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
