---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b963d03d92752f75fbbf73fb3ce9174e1529b61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518130"
---
# <a name="get-device"></a><span data-ttu-id="9528e-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="9528e-103">Get device</span></span>

<span data-ttu-id="9528e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9528e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9528e-105">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="9528e-105">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9528e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9528e-106">Permissions</span></span>
<span data-ttu-id="9528e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9528e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9528e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9528e-109">Permission type</span></span>      | <span data-ttu-id="9528e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9528e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9528e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9528e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9528e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9528e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9528e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9528e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9528e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9528e-114">Not supported.</span></span>    |
|<span data-ttu-id="9528e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9528e-115">Application</span></span> | <span data-ttu-id="9528e-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9528e-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9528e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9528e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="9528e-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="9528e-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="9528e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9528e-119">Optional query parameters</span></span>
<span data-ttu-id="9528e-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9528e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9528e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9528e-121">Request headers</span></span>
| <span data-ttu-id="9528e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9528e-122">Name</span></span>       | <span data-ttu-id="9528e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9528e-123">Type</span></span> | <span data-ttu-id="9528e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9528e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9528e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9528e-125">Authorization</span></span>  | <span data-ttu-id="9528e-126">string</span><span class="sxs-lookup"><span data-stu-id="9528e-126">string</span></span>  | <span data-ttu-id="9528e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9528e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9528e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9528e-129">Request body</span></span>
<span data-ttu-id="9528e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9528e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9528e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9528e-131">Response</span></span>

<span data-ttu-id="9528e-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9528e-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9528e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9528e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9528e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9528e-134">Request</span></span>
<span data-ttu-id="9528e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9528e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9528e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9528e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="9528e-137">C#</span><span class="sxs-lookup"><span data-stu-id="9528e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9528e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9528e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9528e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9528e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9528e-140">Java</span><span class="sxs-lookup"><span data-stu-id="9528e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9528e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9528e-141">Response</span></span>
<span data-ttu-id="9528e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9528e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
