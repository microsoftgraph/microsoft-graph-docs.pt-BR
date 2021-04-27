---
title: Obter dimensões
description: Obtém um objeto dimension no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 656bbd820a3dace3da989f7ae3d4a5115a45289a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045429"
---
# <a name="get-dimensions"></a><span data-ttu-id="88385-103">Obter dimensões</span><span class="sxs-lookup"><span data-stu-id="88385-103">Get dimensions</span></span>

<span data-ttu-id="88385-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88385-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88385-105">Recupere as propriedades e as relações de um **objeto de dimensões** do Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="88385-105">Retrieve the properties and relationships of a **dimensions** object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="88385-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="88385-106">Permissions</span></span>
<span data-ttu-id="88385-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88385-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88385-109">Permission type</span></span> |<span data-ttu-id="88385-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88385-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="88385-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88385-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88385-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88385-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="88385-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="88385-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="88385-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88385-114">Not supported.</span></span>|
|<span data-ttu-id="88385-115">Application</span><span class="sxs-lookup"><span data-stu-id="88385-115">Application</span></span>|<span data-ttu-id="88385-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88385-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88385-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88385-117">HTTP request</span></span>

```
GET /financials/companies/{id}/dimensions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88385-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88385-118">Optional query parameters</span></span>
<span data-ttu-id="88385-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88385-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88385-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88385-120">Request headers</span></span>
|<span data-ttu-id="88385-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88385-121">Header</span></span>|<span data-ttu-id="88385-122">Valor</span><span class="sxs-lookup"><span data-stu-id="88385-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="88385-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88385-123">Authorization</span></span>  |<span data-ttu-id="88385-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88385-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88385-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88385-126">Request body</span></span>
<span data-ttu-id="88385-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88385-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88385-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="88385-128">Response</span></span>
<span data-ttu-id="88385-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **objeto de** dimensões no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88385-129">If successful, this method returns a `200 OK` response code and a **dimensions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88385-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88385-130">Example</span></span>

<span data-ttu-id="88385-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="88385-131">**Request**</span></span>

<span data-ttu-id="88385-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88385-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/dimensions/{id}
```

<span data-ttu-id="88385-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="88385-133">**Response**</span></span>

<span data-ttu-id="88385-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88385-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="88385-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="88385-135">**Note**: The response object shown here might be shortened for readability.</span></span>

```json
{
  "id": "id-value",
  "code": "AREA",
  "displayName": "Area",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```



