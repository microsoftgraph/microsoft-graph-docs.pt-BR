---
title: Obter dispositivo
description: Obtém as propriedades e os relacionamentos de um objeto device.
ms.openlocfilehash: 69c962d6b248738fb03bb3ac39cc37f667ea88e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033595"
---
# <a name="get-device"></a><span data-ttu-id="d9e54-103">Obter dispositivo</span><span class="sxs-lookup"><span data-stu-id="d9e54-103">Get device</span></span>

> <span data-ttu-id="d9e54-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d9e54-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9e54-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d9e54-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9e54-106">Obtém as propriedades e os relacionamentos de um objeto device.</span><span class="sxs-lookup"><span data-stu-id="d9e54-106">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="d9e54-107">Desde que o recurso de **dispositivo** oferece suporte às [extensões](/graph/extensibility-overview), você também pode usar o `GET` operação obter dados de extensão e propriedades personalizadas em uma instância de **dispositivo** .</span><span class="sxs-lookup"><span data-stu-id="d9e54-107">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9e54-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="d9e54-108">Permissions</span></span>
<span data-ttu-id="d9e54-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9e54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d9e54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9e54-111">Permission type</span></span>      | <span data-ttu-id="d9e54-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9e54-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9e54-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9e54-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d9e54-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9e54-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9e54-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9e54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9e54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9e54-116">Not supported.</span></span>    |
|<span data-ttu-id="d9e54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9e54-117">Application</span></span> | <span data-ttu-id="d9e54-118">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e54-118">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9e54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9e54-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9e54-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9e54-120">Optional query parameters</span></span>
<span data-ttu-id="d9e54-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9e54-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d9e54-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9e54-122">Request headers</span></span>
| <span data-ttu-id="d9e54-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d9e54-123">Name</span></span>       | <span data-ttu-id="d9e54-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9e54-124">Type</span></span> | <span data-ttu-id="d9e54-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9e54-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d9e54-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9e54-126">Authorization</span></span>  | <span data-ttu-id="d9e54-127">string</span><span class="sxs-lookup"><span data-stu-id="d9e54-127">string</span></span>  | <span data-ttu-id="d9e54-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9e54-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9e54-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9e54-130">Request body</span></span>
<span data-ttu-id="d9e54-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9e54-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9e54-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9e54-132">Response</span></span>

<span data-ttu-id="d9e54-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9e54-133">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9e54-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9e54-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9e54-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9e54-135">Request</span></span>
<span data-ttu-id="d9e54-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9e54-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="d9e54-137">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="d9e54-137">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="d9e54-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9e54-138">Response</span></span>
<span data-ttu-id="d9e54-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9e54-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d9e54-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="d9e54-142">See also</span></span>

- [<span data-ttu-id="d9e54-143">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="d9e54-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d9e54-144">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="d9e54-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d9e54-145">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="d9e54-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->