---
title: Listar dispositivos
description: 'Recupere uma lista de dispositivos registrados no diretório. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eec732d08a18158570f6826bb9b06208f8d4d4dd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437219"
---
# <a name="list-devices"></a><span data-ttu-id="d63d5-103">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="d63d5-103">List devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d63d5-104">Recupere uma lista de dispositivos registrados no diretório.</span><span class="sxs-lookup"><span data-stu-id="d63d5-104">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d63d5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d63d5-105">Permissions</span></span>
<span data-ttu-id="d63d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d63d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d63d5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d63d5-108">Permission type</span></span>      | <span data-ttu-id="d63d5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d63d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d63d5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d63d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d63d5-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d63d5-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d63d5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d63d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d63d5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d63d5-113">Not supported.</span></span>    |
|<span data-ttu-id="d63d5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d63d5-114">Application</span></span> | <span data-ttu-id="d63d5-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d63d5-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d63d5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d63d5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d63d5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d63d5-117">Optional query parameters</span></span>
<span data-ttu-id="d63d5-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d63d5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d63d5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d63d5-119">Request headers</span></span>
| <span data-ttu-id="d63d5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d63d5-120">Name</span></span>       | <span data-ttu-id="d63d5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d63d5-121">Type</span></span> | <span data-ttu-id="d63d5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d63d5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d63d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d63d5-123">Authorization</span></span>  | <span data-ttu-id="d63d5-124">string</span><span class="sxs-lookup"><span data-stu-id="d63d5-124">string</span></span>  | <span data-ttu-id="d63d5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d63d5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d63d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d63d5-127">Request body</span></span>
<span data-ttu-id="d63d5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d63d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d63d5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d63d5-129">Response</span></span>

<span data-ttu-id="d63d5-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d63d5-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d63d5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d63d5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d63d5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d63d5-132">Request</span></span>
<span data-ttu-id="d63d5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d63d5-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d63d5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d63d5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/beta/devices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d63d5-135">C#</span><span class="sxs-lookup"><span data-stu-id="d63d5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d63d5-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d63d5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d63d5-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d63d5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d63d5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d63d5-138">Response</span></span>
<span data-ttu-id="d63d5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d63d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "accountEnabled": true,
      "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
      "deviceId": "deviceId-value",
      "deviceMetadata": "deviceMetadata-value",
      "displayName" : "displayName-value",
      "id" : "id-value", 
      "operatingSystem" : "operatingSystem-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
