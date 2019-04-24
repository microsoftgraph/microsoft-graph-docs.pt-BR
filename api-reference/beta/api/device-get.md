---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b0bc325620a27d9383b4a12d5f3da970c0c267
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455279"
---
# <a name="get-device"></a><span data-ttu-id="833d9-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="833d9-103">Get device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="833d9-104">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="833d9-104">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="833d9-105">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você também pode usar `GET` a operação para obter propriedades personalizadas e dados de extensão em uma instância de **dispositivo** .</span><span class="sxs-lookup"><span data-stu-id="833d9-105">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="833d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="833d9-106">Permissions</span></span>
<span data-ttu-id="833d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="833d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="833d9-109">Permission type</span></span>      | <span data-ttu-id="833d9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="833d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="833d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="833d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="833d9-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="833d9-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="833d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="833d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="833d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="833d9-114">Not supported.</span></span>    |
|<span data-ttu-id="833d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="833d9-115">Application</span></span> | <span data-ttu-id="833d9-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="833d9-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="833d9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="833d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="833d9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="833d9-118">Optional query parameters</span></span>
<span data-ttu-id="833d9-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="833d9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="833d9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="833d9-120">Request headers</span></span>
| <span data-ttu-id="833d9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="833d9-121">Name</span></span>       | <span data-ttu-id="833d9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="833d9-122">Type</span></span> | <span data-ttu-id="833d9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="833d9-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="833d9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="833d9-124">Authorization</span></span>  | <span data-ttu-id="833d9-125">string</span><span class="sxs-lookup"><span data-stu-id="833d9-125">string</span></span>  | <span data-ttu-id="833d9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="833d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="833d9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="833d9-128">Request body</span></span>
<span data-ttu-id="833d9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="833d9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="833d9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="833d9-130">Response</span></span>

<span data-ttu-id="833d9-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="833d9-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="833d9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="833d9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="833d9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="833d9-133">Request</span></span>
<span data-ttu-id="833d9-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="833d9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="833d9-135">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="833d9-135">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="833d9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="833d9-136">Response</span></span>
<span data-ttu-id="833d9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="833d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="833d9-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="833d9-140">See also</span></span>

- [<span data-ttu-id="833d9-141">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="833d9-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="833d9-142">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="833d9-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="833d9-143">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="833d9-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/device-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
