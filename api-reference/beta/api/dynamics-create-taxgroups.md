---
title: Criar taxGroups
description: Cria um objeto de grupo de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6dfb5d68e18c92de4ecb702707b2fdc67fa5ea19
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365476"
---
# <a name="create-taxgroups"></a><span data-ttu-id="26c3c-103">Criar taxGroups</span><span class="sxs-lookup"><span data-stu-id="26c3c-103">Create taxGroups</span></span>
<span data-ttu-id="26c3c-104">Criar um objeto de grupos de impostos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="26c3c-104">Create a tax groups object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="26c3c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="26c3c-105">Permissions</span></span>
<span data-ttu-id="26c3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26c3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26c3c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26c3c-108">Permission type</span></span> |<span data-ttu-id="26c3c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26c3c-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="26c3c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26c3c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="26c3c-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c3c-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="26c3c-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="26c3c-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="26c3c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26c3c-113">Not supported.</span></span>|
|<span data-ttu-id="26c3c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26c3c-114">Application</span></span>|<span data-ttu-id="26c3c-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c3c-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26c3c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26c3c-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/taxGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26c3c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="26c3c-117">Optional query parameters</span></span>
<span data-ttu-id="26c3c-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="26c3c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26c3c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26c3c-119">Request headers</span></span>

|<span data-ttu-id="26c3c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26c3c-120">Header</span></span>|<span data-ttu-id="26c3c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26c3c-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="26c3c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26c3c-122">Authorization</span></span>  |<span data-ttu-id="26c3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26c3c-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="26c3c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26c3c-125">Content-Type</span></span>  |<span data-ttu-id="26c3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26c3c-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="26c3c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26c3c-127">Request body</span></span>
<span data-ttu-id="26c3c-128">No corpo da solicitação, forneça uma representação JSON de um objeto **taxGroups** .</span><span class="sxs-lookup"><span data-stu-id="26c3c-128">In the request body, supply a JSON representation of a **taxGroups** object.</span></span>

## <a name="response"></a><span data-ttu-id="26c3c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="26c3c-129">Response</span></span>
<span data-ttu-id="26c3c-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **taxGroups** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26c3c-130">If successful, this method returns ```201 Created``` response code and a **taxGroups** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26c3c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26c3c-131">Example</span></span>

<span data-ttu-id="26c3c-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="26c3c-132">**Request**</span></span>

<span data-ttu-id="26c3c-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="26c3c-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/taxGroups
Content-type: application/json

{
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax"
}
```

<span data-ttu-id="26c3c-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="26c3c-134">**Response**</span></span>

<span data-ttu-id="26c3c-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26c3c-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="26c3c-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26c3c-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="26c3c-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26c3c-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}

```
