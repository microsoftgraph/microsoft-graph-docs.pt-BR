---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd253fdfea0b21189bcaf8f32dbd553314e53610
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956398"
---
# <a name="get-device"></a><span data-ttu-id="65039-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="65039-103">Get device</span></span>

<span data-ttu-id="65039-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65039-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65039-105">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="65039-105">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="65039-106">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você também pode usar a `GET` operação para obter propriedades personalizadas e dados de extensão em uma instância de **dispositivo** .</span><span class="sxs-lookup"><span data-stu-id="65039-106">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="65039-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="65039-107">Permissions</span></span>
<span data-ttu-id="65039-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65039-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="65039-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65039-110">Permission type</span></span>      | <span data-ttu-id="65039-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65039-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65039-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65039-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65039-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65039-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65039-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65039-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65039-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65039-115">Not supported.</span></span>    |
|<span data-ttu-id="65039-116">Application</span><span class="sxs-lookup"><span data-stu-id="65039-116">Application</span></span> | <span data-ttu-id="65039-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65039-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65039-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65039-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65039-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65039-119">Optional query parameters</span></span>
<span data-ttu-id="65039-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65039-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="65039-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65039-121">Request headers</span></span>
| <span data-ttu-id="65039-122">Nome</span><span class="sxs-lookup"><span data-stu-id="65039-122">Name</span></span>       | <span data-ttu-id="65039-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="65039-123">Type</span></span> | <span data-ttu-id="65039-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="65039-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65039-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="65039-125">Authorization</span></span>  | <span data-ttu-id="65039-126">string</span><span class="sxs-lookup"><span data-stu-id="65039-126">string</span></span>  | <span data-ttu-id="65039-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65039-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65039-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65039-129">Request body</span></span>
<span data-ttu-id="65039-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65039-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65039-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="65039-131">Response</span></span>

<span data-ttu-id="65039-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65039-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65039-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65039-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65039-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65039-134">Request</span></span>
<span data-ttu-id="65039-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65039-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65039-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="65039-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="65039-137">C#</span><span class="sxs-lookup"><span data-stu-id="65039-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65039-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65039-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65039-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65039-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65039-140">Java</span><span class="sxs-lookup"><span data-stu-id="65039-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="65039-141">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="65039-141">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="65039-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="65039-142">Response</span></span>
<span data-ttu-id="65039-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65039-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="65039-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="65039-146">See also</span></span>

- [<span data-ttu-id="65039-147">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="65039-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="65039-148">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="65039-148">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="65039-149">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="65039-149">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
