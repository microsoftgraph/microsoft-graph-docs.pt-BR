---
title: 'cloudPcDeviceImage: getSourceImages'
description: Exibir uma lista de todos os recursos de imagem gerenciada de suas assinaturas do Azure. Essas imagens de origem podem ser carregadas e usadas em PCs na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1ddd7fdef827328f6f72b52af5a992e9f0d69653
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872776"
---
# <a name="cloudpcdeviceimage-getsourceimages"></a><span data-ttu-id="c9dd4-104">cloudPcDeviceImage: getSourceImages</span><span class="sxs-lookup"><span data-stu-id="c9dd4-104">cloudPcDeviceImage: getSourceImages</span></span>

<span data-ttu-id="c9dd4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9dd4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9dd4-106">Obter [objetos cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="c9dd4-106">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span> <span data-ttu-id="c9dd4-107">Exibir uma lista de todos os recursos de imagem gerenciada de suas assinaturas do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c9dd4-107">View a list of all the managed image resources from your Azure Active Directory subscriptions.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="c9dd4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9dd4-108">Permissions</span></span>

<span data-ttu-id="c9dd4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9dd4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9dd4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9dd4-111">Permission type</span></span>|<span data-ttu-id="c9dd4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9dd4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9dd4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9dd4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9dd4-114">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9dd4-114">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c9dd4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9dd4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9dd4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9dd4-116">Not supported.</span></span>|
|<span data-ttu-id="c9dd4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9dd4-117">Application</span></span>|<span data-ttu-id="c9dd4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9dd4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9dd4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9dd4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

## <a name="request-headers"></a><span data-ttu-id="c9dd4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9dd4-120">Request headers</span></span>

|<span data-ttu-id="c9dd4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c9dd4-121">Name</span></span>|<span data-ttu-id="c9dd4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9dd4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c9dd4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9dd4-123">Authorization</span></span>|<span data-ttu-id="c9dd4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9dd4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9dd4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9dd4-126">Request body</span></span>

<span data-ttu-id="c9dd4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9dd4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9dd4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9dd4-128">Response</span></span>

<span data-ttu-id="c9dd4-129">Se bem-sucedida, esta função retorna um código de resposta e uma coleção `200 OK` [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9dd4-129">If successful, this function returns a `200 OK` response code and a [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9dd4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c9dd4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9dd4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9dd4-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c9dd4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9dd4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcdeviceimage_getsourceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```
# <a name="c"></a>[<span data-ttu-id="c9dd4-133">C#</span><span class="sxs-lookup"><span data-stu-id="c9dd4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcdeviceimage-getsourceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9dd4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9dd4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcdeviceimage-getsourceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9dd4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9dd4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcdeviceimage-getsourceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9dd4-136">Java</span><span class="sxs-lookup"><span data-stu-id="c9dd4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcdeviceimage-getsourceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c9dd4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9dd4-137">Response</span></span>

<span data-ttu-id="c9dd4-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c9dd4-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcSourceDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
      "id": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "displayName": "Display Name value"
    }
  ]
}
```
