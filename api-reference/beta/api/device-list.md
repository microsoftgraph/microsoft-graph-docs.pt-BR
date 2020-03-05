---
title: Listar dispositivos
description: 'Recupere uma lista de dispositivos registrados no diretório. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 01fea91712c9112165df5709321c00d26269ddab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435728"
---
# <a name="list-devices"></a><span data-ttu-id="56ee1-103">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="56ee1-103">List devices</span></span>

<span data-ttu-id="56ee1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="56ee1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56ee1-105">Recupere uma lista de dispositivos registrados no diretório.</span><span class="sxs-lookup"><span data-stu-id="56ee1-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="56ee1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="56ee1-106">Permissions</span></span>
<span data-ttu-id="56ee1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ee1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="56ee1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56ee1-109">Permission type</span></span>      | <span data-ttu-id="56ee1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56ee1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56ee1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56ee1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="56ee1-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56ee1-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56ee1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56ee1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56ee1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56ee1-114">Not supported.</span></span>    |
|<span data-ttu-id="56ee1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56ee1-115">Application</span></span> | <span data-ttu-id="56ee1-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56ee1-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56ee1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56ee1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56ee1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56ee1-118">Optional query parameters</span></span>
<span data-ttu-id="56ee1-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56ee1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56ee1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56ee1-120">Request headers</span></span>
| <span data-ttu-id="56ee1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="56ee1-121">Name</span></span>       | <span data-ttu-id="56ee1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="56ee1-122">Type</span></span> | <span data-ttu-id="56ee1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ee1-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56ee1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="56ee1-124">Authorization</span></span>  | <span data-ttu-id="56ee1-125">string</span><span class="sxs-lookup"><span data-stu-id="56ee1-125">string</span></span>  | <span data-ttu-id="56ee1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56ee1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56ee1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56ee1-128">Request body</span></span>
<span data-ttu-id="56ee1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56ee1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56ee1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ee1-130">Response</span></span>

<span data-ttu-id="56ee1-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56ee1-131">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56ee1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56ee1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56ee1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56ee1-133">Request</span></span>
<span data-ttu-id="56ee1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56ee1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56ee1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="56ee1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="56ee1-136">C#</span><span class="sxs-lookup"><span data-stu-id="56ee1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56ee1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56ee1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56ee1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56ee1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="56ee1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ee1-139">Response</span></span>
<span data-ttu-id="56ee1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56ee1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
