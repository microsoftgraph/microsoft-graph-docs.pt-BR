---
title: Obter configurações
description: Recupere configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 675e0c41e0aa9605b0a6088e13be78e9d52d57be
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895716"
---
# <a name="get-settings"></a><span data-ttu-id="badfa-103">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="badfa-103">Get settings</span></span>

<span data-ttu-id="badfa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="badfa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="badfa-105">Recupere configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="badfa-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="badfa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="badfa-106">Permissions</span></span>
<span data-ttu-id="badfa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="badfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="badfa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="badfa-109">Permission type</span></span> | <span data-ttu-id="badfa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="badfa-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="badfa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="badfa-111">Delegated (work or school account)</span></span>| <span data-ttu-id="badfa-112">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="badfa-112">Users.Read.All</span></span> |
|<span data-ttu-id="badfa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="badfa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="badfa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="badfa-114">Not Supported.</span></span>|
|<span data-ttu-id="badfa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="badfa-115">Application</span></span>|<span data-ttu-id="badfa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="badfa-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="badfa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="badfa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="badfa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="badfa-118">Optional query parameters</span></span>
<span data-ttu-id="badfa-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="badfa-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="badfa-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="badfa-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="badfa-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="badfa-121">Request headers</span></span>
| <span data-ttu-id="badfa-122">Nome</span><span class="sxs-lookup"><span data-stu-id="badfa-122">Name</span></span>      |<span data-ttu-id="badfa-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="badfa-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="badfa-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="badfa-124">Authorization</span></span> | <span data-ttu-id="badfa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="badfa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="badfa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="badfa-127">Request body</span></span>
<span data-ttu-id="badfa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="badfa-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="badfa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="badfa-129">Response</span></span>
<span data-ttu-id="badfa-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printSettings](../resources/printsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="badfa-130">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="badfa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="badfa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="badfa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="badfa-132">Request</span></span>
<span data-ttu-id="badfa-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="badfa-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}-->
```http
GET https://graph.microsoft.com/beta/print/settings
```
##### <a name="response"></a><span data-ttu-id="badfa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="badfa-134">Response</span></span>
<span data-ttu-id="badfa-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="badfa-135">The following is an example of the response.</span></span>
><span data-ttu-id="badfa-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="badfa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 144

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->