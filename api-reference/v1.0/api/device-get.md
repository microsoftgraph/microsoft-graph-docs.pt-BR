---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
ms.openlocfilehash: 07ee10ccc6f3cfb7649df2cb3711bfff24115036
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006954"
---
# <a name="get-device"></a><span data-ttu-id="2c194-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="2c194-103">Get device</span></span>

<span data-ttu-id="2c194-104">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="2c194-104">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c194-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c194-105">Permissions</span></span>
<span data-ttu-id="2c194-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2c194-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c194-108">Permission type</span></span>      | <span data-ttu-id="2c194-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c194-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c194-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c194-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c194-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c194-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c194-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c194-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c194-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c194-113">Not supported.</span></span>    |
|<span data-ttu-id="2c194-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c194-114">Application</span></span> | <span data-ttu-id="2c194-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c194-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c194-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c194-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="2c194-117">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="2c194-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2c194-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2c194-118">Optional query parameters</span></span>
<span data-ttu-id="2c194-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c194-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c194-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c194-120">Request headers</span></span>
| <span data-ttu-id="2c194-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2c194-121">Name</span></span>       | <span data-ttu-id="2c194-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c194-122">Type</span></span> | <span data-ttu-id="2c194-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c194-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2c194-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c194-124">Authorization</span></span>  | <span data-ttu-id="2c194-125">string</span><span class="sxs-lookup"><span data-stu-id="2c194-125">string</span></span>  | <span data-ttu-id="2c194-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c194-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c194-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c194-128">Request body</span></span>
<span data-ttu-id="2c194-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c194-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c194-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c194-130">Response</span></span>

<span data-ttu-id="2c194-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c194-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c194-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c194-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c194-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c194-133">Request</span></span>
<span data-ttu-id="2c194-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c194-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="2c194-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c194-135">Response</span></span>
<span data-ttu-id="2c194-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c194-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
