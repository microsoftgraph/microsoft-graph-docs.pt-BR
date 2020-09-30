---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 94bc3fe7a5485a39903a3e30bb38b76e9021a31f
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48311998"
---
# <a name="get-device"></a><span data-ttu-id="ddce9-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="ddce9-103">Get device</span></span>

<span data-ttu-id="ddce9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddce9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddce9-105">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="ddce9-105">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="ddce9-106">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você também pode usar a `GET` operação para obter propriedades personalizadas e dados de extensão em uma instância de **dispositivo** .</span><span class="sxs-lookup"><span data-stu-id="ddce9-106">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddce9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddce9-107">Permissions</span></span>
<span data-ttu-id="ddce9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ddce9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddce9-110">Permission type</span></span>      | <span data-ttu-id="ddce9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddce9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddce9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddce9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ddce9-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddce9-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ddce9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddce9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddce9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddce9-115">Not supported.</span></span>    |
|<span data-ttu-id="ddce9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddce9-116">Application</span></span> | <span data-ttu-id="ddce9-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddce9-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddce9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddce9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ddce9-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ddce9-119">Optional query parameters</span></span>
<span data-ttu-id="ddce9-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ddce9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ddce9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddce9-121">Request headers</span></span>
| <span data-ttu-id="ddce9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ddce9-122">Name</span></span>       | <span data-ttu-id="ddce9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddce9-123">Type</span></span> | <span data-ttu-id="ddce9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddce9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ddce9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddce9-125">Authorization</span></span>  | <span data-ttu-id="ddce9-126">string</span><span class="sxs-lookup"><span data-stu-id="ddce9-126">string</span></span>  | <span data-ttu-id="ddce9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddce9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddce9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddce9-129">Request body</span></span>
<span data-ttu-id="ddce9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddce9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddce9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddce9-131">Response</span></span>

<span data-ttu-id="ddce9-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddce9-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ddce9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddce9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddce9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddce9-134">Request</span></span>
<span data-ttu-id="ddce9-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddce9-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddce9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddce9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="ddce9-137">C#</span><span class="sxs-lookup"><span data-stu-id="ddce9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddce9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddce9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddce9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddce9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="ddce9-140">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="ddce9-140">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="ddce9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddce9-141">Response</span></span>
<span data-ttu-id="ddce9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddce9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 322

{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="ddce9-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="ddce9-145">See also</span></span>

- [<span data-ttu-id="ddce9-146">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="ddce9-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ddce9-147">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="ddce9-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ddce9-148">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="ddce9-148">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->