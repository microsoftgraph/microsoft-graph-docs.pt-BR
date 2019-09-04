---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e7aa809cfd2d597e7ac284e5daf4e052fd4282f5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718303"
---
# <a name="get-device"></a><span data-ttu-id="dbc66-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="dbc66-103">Get device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbc66-104">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="dbc66-104">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="dbc66-105">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você também pode usar `GET` a operação para obter propriedades personalizadas e dados de extensão em uma instância de **dispositivo** .</span><span class="sxs-lookup"><span data-stu-id="dbc66-105">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbc66-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbc66-106">Permissions</span></span>
<span data-ttu-id="dbc66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbc66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dbc66-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbc66-109">Permission type</span></span>      | <span data-ttu-id="dbc66-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbc66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbc66-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbc66-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbc66-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dbc66-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dbc66-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbc66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbc66-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbc66-114">Not supported.</span></span>    |
|<span data-ttu-id="dbc66-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbc66-115">Application</span></span> | <span data-ttu-id="dbc66-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbc66-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbc66-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbc66-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dbc66-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dbc66-118">Optional query parameters</span></span>
<span data-ttu-id="dbc66-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dbc66-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dbc66-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc66-120">Request headers</span></span>
| <span data-ttu-id="dbc66-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dbc66-121">Name</span></span>       | <span data-ttu-id="dbc66-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbc66-122">Type</span></span> | <span data-ttu-id="dbc66-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbc66-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dbc66-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbc66-124">Authorization</span></span>  | <span data-ttu-id="dbc66-125">string</span><span class="sxs-lookup"><span data-stu-id="dbc66-125">string</span></span>  | <span data-ttu-id="dbc66-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbc66-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbc66-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc66-128">Request body</span></span>
<span data-ttu-id="dbc66-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbc66-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbc66-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbc66-130">Response</span></span>

<span data-ttu-id="dbc66-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbc66-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dbc66-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbc66-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbc66-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc66-133">Request</span></span>
<span data-ttu-id="dbc66-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbc66-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dbc66-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbc66-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbc66-136">C#</span><span class="sxs-lookup"><span data-stu-id="dbc66-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbc66-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbc66-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbc66-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dbc66-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="dbc66-139">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="dbc66-139">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="dbc66-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbc66-140">Response</span></span>
<span data-ttu-id="dbc66-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbc66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dbc66-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="dbc66-144">See also</span></span>

- [<span data-ttu-id="dbc66-145">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="dbc66-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="dbc66-146">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="dbc66-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="dbc66-147">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="dbc66-147">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
