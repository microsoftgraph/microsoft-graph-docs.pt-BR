---
title: Criar unitsOfMeasure
description: Cria um objeto de unidade de medida no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 41c312a7b118dbe161c56d4eb226ef390d0d3d1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956538"
---
# <a name="create-unitsofmeasure"></a><span data-ttu-id="9de0a-103">Criar unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="9de0a-103">Create unitsOfMeasure</span></span>
<span data-ttu-id="9de0a-104">Criar um objeto de unidades de medida no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="9de0a-104">Create a units of measure object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9de0a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9de0a-105">Permissions</span></span>
<span data-ttu-id="9de0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9de0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9de0a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9de0a-108">Permission type</span></span> |<span data-ttu-id="9de0a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9de0a-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9de0a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9de0a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9de0a-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de0a-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9de0a-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="9de0a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9de0a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9de0a-113">Not supported.</span></span>|
|<span data-ttu-id="9de0a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9de0a-114">Application</span></span>|<span data-ttu-id="9de0a-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de0a-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9de0a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9de0a-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/unitsOfMeasure
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9de0a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9de0a-117">Optional query parameters</span></span>
<span data-ttu-id="9de0a-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9de0a-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9de0a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9de0a-119">Request headers</span></span>
|<span data-ttu-id="9de0a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9de0a-120">Header</span></span>|<span data-ttu-id="9de0a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9de0a-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="9de0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9de0a-122">Authorization</span></span>  |<span data-ttu-id="9de0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9de0a-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9de0a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9de0a-125">Content-Type</span></span>  |<span data-ttu-id="9de0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9de0a-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="9de0a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9de0a-127">Request body</span></span>
<span data-ttu-id="9de0a-128">No corpo da solicitação, forneça uma representação JSON de um objeto **unitsOfMeasure** .</span><span class="sxs-lookup"><span data-stu-id="9de0a-128">In the request body, supply a JSON representation of a **unitsOfMeasure** object.</span></span>

## <a name="response"></a><span data-ttu-id="9de0a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9de0a-129">Response</span></span>
<span data-ttu-id="9de0a-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **unitsOfMeasure** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9de0a-130">If successful, this method returns ```201 Created``` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9de0a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9de0a-131">Example</span></span>

<span data-ttu-id="9de0a-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="9de0a-132">**Request**</span></span>

<span data-ttu-id="9de0a-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9de0a-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/unitsOfMeasure
Content-type: application/json

{
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA"
}
```

<span data-ttu-id="9de0a-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="9de0a-134">**Response**</span></span>

<span data-ttu-id="9de0a-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9de0a-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="9de0a-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9de0a-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9de0a-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9de0a-137">All the properties will be returned from an actual call.</span></span>

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

