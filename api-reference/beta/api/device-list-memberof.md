---
title: Listar grupos de dispositivos
description: Obter grupos dos quais este dispositivo é membro direto. Essa operação não é transitiva.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9a0e7a3ec93766b8b517b558a3bfa5b6778d45c7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321461"
---
# <a name="list-device-groups"></a><span data-ttu-id="d36b3-104">Listar grupos de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d36b3-104">List device groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d36b3-105">Obter grupos dos quais este dispositivo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="d36b3-105">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="d36b3-106">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="d36b3-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d36b3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d36b3-107">Permissions</span></span>

<span data-ttu-id="d36b3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d36b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d36b3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d36b3-110">Permission type</span></span>      | <span data-ttu-id="d36b3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d36b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d36b3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d36b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d36b3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d36b3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d36b3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d36b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d36b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d36b3-115">Not supported.</span></span>    |
|<span data-ttu-id="d36b3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d36b3-116">Application</span></span> | <span data-ttu-id="d36b3-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d36b3-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d36b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d36b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d36b3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d36b3-119">Optional query parameters</span></span>
<span data-ttu-id="d36b3-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d36b3-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d36b3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d36b3-121">Request headers</span></span>
| <span data-ttu-id="d36b3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d36b3-122">Header</span></span>       | <span data-ttu-id="d36b3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d36b3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d36b3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d36b3-124">Authorization</span></span>  | <span data-ttu-id="d36b3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d36b3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d36b3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d36b3-127">Accept</span></span>  | <span data-ttu-id="d36b3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d36b3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d36b3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d36b3-129">Request body</span></span>
<span data-ttu-id="d36b3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d36b3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d36b3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d36b3-131">Response</span></span>

<span data-ttu-id="d36b3-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d36b3-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d36b3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d36b3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d36b3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d36b3-134">Request</span></span>

<span data-ttu-id="d36b3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d36b3-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d36b3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d36b3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d36b3-137">C#</span><span class="sxs-lookup"><span data-stu-id="d36b3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d36b3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d36b3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d36b3-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d36b3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d36b3-140">Java</span><span class="sxs-lookup"><span data-stu-id="d36b3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d36b3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d36b3-141">Response</span></span>
<span data-ttu-id="d36b3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d36b3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
