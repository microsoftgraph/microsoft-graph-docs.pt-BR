---
title: Listar dispositivos
description: Recupera uma lista de objetos de dispositivos registrados na organização.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 432d7e263faab60a95084ca3d7aef6cb42f5884d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973404"
---
# <a name="list-devices"></a><span data-ttu-id="1b569-103">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="1b569-103">List devices</span></span>

<span data-ttu-id="1b569-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b569-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b569-105">Recupera uma lista de objetos de dispositivos registrados na organização.</span><span class="sxs-lookup"><span data-stu-id="1b569-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b569-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b569-106">Permissions</span></span>
<span data-ttu-id="1b569-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b569-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1b569-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b569-109">Permission type</span></span>      | <span data-ttu-id="1b569-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b569-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b569-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b569-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b569-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b569-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1b569-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b569-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b569-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b569-114">Not supported.</span></span>    |
|<span data-ttu-id="1b569-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b569-115">Application</span></span> | <span data-ttu-id="1b569-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b569-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b569-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b569-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b569-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b569-118">Optional query parameters</span></span>
<span data-ttu-id="1b569-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b569-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1b569-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b569-120">Request headers</span></span>
| <span data-ttu-id="1b569-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1b569-121">Name</span></span>       | <span data-ttu-id="1b569-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b569-122">Type</span></span> | <span data-ttu-id="1b569-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b569-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1b569-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b569-124">Authorization</span></span>  | <span data-ttu-id="1b569-125">string</span><span class="sxs-lookup"><span data-stu-id="1b569-125">string</span></span>  | <span data-ttu-id="1b569-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b569-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b569-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b569-128">Request body</span></span>
<span data-ttu-id="1b569-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b569-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b569-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b569-130">Response</span></span>

<span data-ttu-id="1b569-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b569-131">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b569-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b569-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b569-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b569-133">Request</span></span>
<span data-ttu-id="1b569-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b569-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b569-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b569-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="1b569-136">C#</span><span class="sxs-lookup"><span data-stu-id="1b569-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b569-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b569-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b569-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b569-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b569-139">Java</span><span class="sxs-lookup"><span data-stu-id="1b569-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1b569-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b569-140">Response</span></span>
<span data-ttu-id="1b569-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b569-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

