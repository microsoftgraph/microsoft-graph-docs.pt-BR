---
title: Listar userSettings
description: Recupere uma lista de objetos cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 2a5665a1e1043296f3814bdc301c8f3c6b339655
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208372"
---
# <a name="list-usersettings"></a><span data-ttu-id="46429-103">Listar userSettings</span><span class="sxs-lookup"><span data-stu-id="46429-103">List userSettings</span></span>

<span data-ttu-id="46429-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46429-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46429-105">Recupere uma lista de [objetos cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="46429-105">Retrieve a list of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="46429-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46429-106">Permissions</span></span>

<span data-ttu-id="46429-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46429-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46429-109">Permission type</span></span>|<span data-ttu-id="46429-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46429-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46429-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46429-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46429-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46429-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="46429-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46429-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46429-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46429-114">Not supported.</span></span>|
|<span data-ttu-id="46429-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46429-115">Application</span></span>|<span data-ttu-id="46429-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46429-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46429-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46429-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46429-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46429-118">Optional query parameters</span></span>

<span data-ttu-id="46429-119">Este método oferece suporte `$select` aos `$filter` parâmetros de consulta , e `$expand` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46429-119">This method the supports `$select`, `$filter`, and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="46429-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="46429-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="46429-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46429-121">Request headers</span></span>

| <span data-ttu-id="46429-122">Nome</span><span class="sxs-lookup"><span data-stu-id="46429-122">Name</span></span>          | <span data-ttu-id="46429-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="46429-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="46429-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="46429-124">Authorization</span></span> | <span data-ttu-id="46429-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46429-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46429-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46429-127">Request body</span></span>

<span data-ttu-id="46429-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46429-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46429-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46429-129">Response</span></span>

<span data-ttu-id="46429-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcUserSetting](../resources/cloudpcusersetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46429-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46429-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46429-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46429-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46429-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="46429-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="46429-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
```
# <a name="c"></a>[<span data-ttu-id="46429-134">C#</span><span class="sxs-lookup"><span data-stu-id="46429-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46429-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46429-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46429-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46429-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46429-137">Java</span><span class="sxs-lookup"><span data-stu-id="46429-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="46429-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="46429-138">Response</span></span>
><span data-ttu-id="46429-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="46429-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcUserSetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcUserSetting",
      "id": "556092f8-92f8-5560-f892-6055f8926055",
      "displayName": "Test1",
      "selfServiceEnabled": true,
      "localAdminEnabled": false,
      "lastModifiedDateTime": "2021-02-01T10:29:57Z",
      "createdDateTime": "2021-02-01T10:29:57Z"
    }
  ]
}
```
