---
title: Listar dispositivos
description: Recupera uma lista de objetos de dispositivos registrados na organização.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 25812f63b85bcc6e9c69dc77433aa7c4c7bb78af
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276297"
---
# <a name="list-devices"></a><span data-ttu-id="b1173-103">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="b1173-103">List devices</span></span>

<span data-ttu-id="b1173-104">Recupera uma lista de objetos de dispositivos registrados na organização.</span><span class="sxs-lookup"><span data-stu-id="b1173-104">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1173-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1173-105">Permissions</span></span>
<span data-ttu-id="b1173-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b1173-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1173-108">Permission type</span></span>      | <span data-ttu-id="b1173-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1173-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1173-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1173-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1173-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1173-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b1173-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1173-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1173-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1173-113">Not supported.</span></span>    |
|<span data-ttu-id="b1173-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1173-114">Application</span></span> | <span data-ttu-id="b1173-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1173-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1173-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1173-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1173-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1173-117">Optional query parameters</span></span>
<span data-ttu-id="b1173-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1173-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1173-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1173-119">Request headers</span></span>
| <span data-ttu-id="b1173-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b1173-120">Name</span></span>       | <span data-ttu-id="b1173-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1173-121">Type</span></span> | <span data-ttu-id="b1173-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1173-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1173-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1173-123">Authorization</span></span>  | <span data-ttu-id="b1173-124">string</span><span class="sxs-lookup"><span data-stu-id="b1173-124">string</span></span>  | <span data-ttu-id="b1173-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1173-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1173-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1173-127">Request body</span></span>
<span data-ttu-id="b1173-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1173-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1173-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1173-129">Response</span></span>

<span data-ttu-id="b1173-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1173-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1173-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1173-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1173-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1173-132">Request</span></span>
<span data-ttu-id="b1173-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1173-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="b1173-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1173-134">Response</span></span>
<span data-ttu-id="b1173-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1173-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b1173-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b1173-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b1173-139">C#</span><span class="sxs-lookup"><span data-stu-id="b1173-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_devices-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1173-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1173-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_devices-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b1173-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b1173-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_devices-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
