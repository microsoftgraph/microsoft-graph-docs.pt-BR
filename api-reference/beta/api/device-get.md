---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d6bf4e1060c723c1cba9d77811d76f8be20518bc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261009"
---
# <a name="get-device"></a><span data-ttu-id="5b4fb-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="5b4fb-103">Get device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b4fb-104">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="5b4fb-104">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="5b4fb-105">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você também pode usar `GET` a operação para obter propriedades personalizadas e dados de extensão em uma instância de **dispositivo** .</span><span class="sxs-lookup"><span data-stu-id="5b4fb-105">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b4fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b4fb-106">Permissions</span></span>
<span data-ttu-id="5b4fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b4fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5b4fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b4fb-109">Permission type</span></span>      | <span data-ttu-id="5b4fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b4fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b4fb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b4fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b4fb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5b4fb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b4fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b4fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b4fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b4fb-114">Not supported.</span></span>    |
|<span data-ttu-id="5b4fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b4fb-115">Application</span></span> | <span data-ttu-id="5b4fb-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4fb-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b4fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b4fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b4fb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b4fb-118">Optional query parameters</span></span>
<span data-ttu-id="5b4fb-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b4fb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5b4fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4fb-120">Request headers</span></span>
| <span data-ttu-id="5b4fb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5b4fb-121">Name</span></span>       | <span data-ttu-id="5b4fb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b4fb-122">Type</span></span> | <span data-ttu-id="5b4fb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b4fb-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5b4fb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b4fb-124">Authorization</span></span>  | <span data-ttu-id="5b4fb-125">string</span><span class="sxs-lookup"><span data-stu-id="5b4fb-125">string</span></span>  | <span data-ttu-id="5b4fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b4fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b4fb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4fb-128">Request body</span></span>
<span data-ttu-id="5b4fb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b4fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b4fb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b4fb-130">Response</span></span>

<span data-ttu-id="5b4fb-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b4fb-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b4fb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b4fb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b4fb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4fb-133">Request</span></span>
<span data-ttu-id="5b4fb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b4fb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="5b4fb-135">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="5b4fb-135">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="5b4fb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b4fb-136">Response</span></span>
<span data-ttu-id="5b4fb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b4fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b4fb-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5b4fb-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b4fb-141">C#</span><span class="sxs-lookup"><span data-stu-id="5b4fb-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b4fb-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b4fb-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_device-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5b4fb-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5b4fb-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_device-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="5b4fb-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="5b4fb-144">See also</span></span>

- [<span data-ttu-id="5b4fb-145">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="5b4fb-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5b4fb-146">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="5b4fb-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5b4fb-147">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="5b4fb-147">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/device-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/device-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
