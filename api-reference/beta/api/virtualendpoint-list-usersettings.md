---
title: Listar userSettings
description: Recupere uma lista de objetos cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6d953baaf3d071ca999031bfd5ae07dcfe378106
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993638"
---
# <a name="list-usersettings"></a><span data-ttu-id="29239-103">Listar userSettings</span><span class="sxs-lookup"><span data-stu-id="29239-103">List userSettings</span></span>

<span data-ttu-id="29239-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29239-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29239-105">Recupere uma lista de [objetos cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="29239-105">Retrieve a list of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="29239-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="29239-106">Permissions</span></span>

<span data-ttu-id="29239-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29239-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29239-109">Permission type</span></span>|<span data-ttu-id="29239-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29239-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29239-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29239-111">Delegated (work or school account)</span></span>|<span data-ttu-id="29239-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29239-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="29239-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29239-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29239-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29239-114">Not supported.</span></span>|
|<span data-ttu-id="29239-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29239-115">Application</span></span>|<span data-ttu-id="29239-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29239-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29239-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29239-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29239-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="29239-118">Optional query parameters</span></span>

<span data-ttu-id="29239-119">Este método oferece suporte `$select` aos `$filter` parâmetros de consulta , e `$expand` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="29239-119">This method the supports `$select`, `$filter`, and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="29239-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="29239-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="29239-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29239-121">Request headers</span></span>

| <span data-ttu-id="29239-122">Nome</span><span class="sxs-lookup"><span data-stu-id="29239-122">Name</span></span>          | <span data-ttu-id="29239-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="29239-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="29239-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="29239-124">Authorization</span></span> | <span data-ttu-id="29239-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29239-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29239-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29239-127">Request body</span></span>

<span data-ttu-id="29239-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29239-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29239-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="29239-129">Response</span></span>

<span data-ttu-id="29239-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcUserSetting](../resources/cloudpcusersetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29239-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29239-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29239-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29239-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29239-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
```


### <a name="response"></a><span data-ttu-id="29239-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="29239-133">Response</span></span>
><span data-ttu-id="29239-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="29239-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
