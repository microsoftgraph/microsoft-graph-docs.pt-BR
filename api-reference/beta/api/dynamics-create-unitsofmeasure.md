---
title: Criar unitsOfMeasure
description: Cria um objeto de unidade de medida no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c1cf9e8c2d60c2af6ed20a2203b58c9edadd662f
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791866"
---
# <a name="create-unitsofmeasure"></a><span data-ttu-id="0ccef-103">Criar unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="0ccef-103">Create unitsOfMeasure</span></span>
<span data-ttu-id="0ccef-104">Criar um objeto de unidades de medida no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="0ccef-104">Create a units of measure object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ccef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ccef-105">Permissions</span></span>
<span data-ttu-id="0ccef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ccef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ccef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ccef-108">Permission type</span></span> |<span data-ttu-id="0ccef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ccef-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="0ccef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ccef-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0ccef-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ccef-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="0ccef-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="0ccef-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0ccef-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ccef-113">Not supported.</span></span>|
|<span data-ttu-id="0ccef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ccef-114">Application</span></span>|<span data-ttu-id="0ccef-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ccef-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ccef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ccef-116">HTTP request</span></span>
```
POST /financials/companies/{id}/unitsOfMeasure
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ccef-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ccef-117">Optional query parameters</span></span>
<span data-ttu-id="0ccef-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ccef-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ccef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ccef-119">Request headers</span></span>
|<span data-ttu-id="0ccef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ccef-120">Header</span></span>|<span data-ttu-id="0ccef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0ccef-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="0ccef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ccef-122">Authorization</span></span>  |<span data-ttu-id="0ccef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ccef-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="0ccef-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ccef-125">Content-Type</span></span>  |<span data-ttu-id="0ccef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ccef-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="0ccef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ccef-127">Request body</span></span>
<span data-ttu-id="0ccef-128">No corpo da solicitação, forneça uma representação JSON de um objeto **unitsOfMeasure** .</span><span class="sxs-lookup"><span data-stu-id="0ccef-128">In the request body, supply a JSON representation of a **unitsOfMeasure** object.</span></span>

## <a name="response"></a><span data-ttu-id="0ccef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ccef-129">Response</span></span>
<span data-ttu-id="0ccef-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **unitsOfMeasure** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ccef-130">If successful, this method returns ```201 Created``` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ccef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ccef-131">Example</span></span>

<span data-ttu-id="0ccef-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="0ccef-132">**Request**</span></span>

<span data-ttu-id="0ccef-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ccef-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure
Content-type: application/json

{
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA"
}
```

<span data-ttu-id="0ccef-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="0ccef-134">**Response**</span></span>

<span data-ttu-id="0ccef-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ccef-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="0ccef-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0ccef-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0ccef-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ccef-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}

```

