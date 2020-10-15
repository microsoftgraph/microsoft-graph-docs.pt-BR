---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: daf46d80400601cec87a5c6f89e4166f6c86b360
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461535"
---
# <a name="get-device"></a><span data-ttu-id="18be3-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="18be3-103">Get device</span></span>

<span data-ttu-id="18be3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18be3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18be3-105">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="18be3-105">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="18be3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="18be3-106">Permissions</span></span>
<span data-ttu-id="18be3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18be3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="18be3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18be3-109">Permission type</span></span>      | <span data-ttu-id="18be3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18be3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18be3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18be3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18be3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18be3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18be3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18be3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18be3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18be3-114">Not supported.</span></span>    |
|<span data-ttu-id="18be3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18be3-115">Application</span></span> | <span data-ttu-id="18be3-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be3-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18be3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18be3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="18be3-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="18be3-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="18be3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="18be3-119">Optional query parameters</span></span>
<span data-ttu-id="18be3-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="18be3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18be3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18be3-121">Request headers</span></span>
| <span data-ttu-id="18be3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="18be3-122">Name</span></span>       | <span data-ttu-id="18be3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="18be3-123">Type</span></span> | <span data-ttu-id="18be3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="18be3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18be3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="18be3-125">Authorization</span></span>  | <span data-ttu-id="18be3-126">string</span><span class="sxs-lookup"><span data-stu-id="18be3-126">string</span></span>  | <span data-ttu-id="18be3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18be3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18be3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18be3-129">Request body</span></span>
<span data-ttu-id="18be3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18be3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18be3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="18be3-131">Response</span></span>

<span data-ttu-id="18be3-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18be3-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18be3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18be3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18be3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18be3-134">Request</span></span>
<span data-ttu-id="18be3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18be3-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18be3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="18be3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="18be3-137">C#</span><span class="sxs-lookup"><span data-stu-id="18be3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18be3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18be3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18be3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18be3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18be3-140">Java</span><span class="sxs-lookup"><span data-stu-id="18be3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="18be3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="18be3-141">Response</span></span>
<span data-ttu-id="18be3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18be3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
