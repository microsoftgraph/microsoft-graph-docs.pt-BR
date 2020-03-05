---
title: Criar taxGroups
description: Cria um objeto de grupo de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8bc45dfbb7efe2d2f5fcc3ab33af38331621445b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431145"
---
# <a name="create-taxgroups"></a><span data-ttu-id="fa61e-103">Criar taxGroups</span><span class="sxs-lookup"><span data-stu-id="fa61e-103">Create taxGroups</span></span>

<span data-ttu-id="fa61e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa61e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa61e-105">Criar um objeto de grupos de impostos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="fa61e-105">Create a tax groups object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa61e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa61e-106">Permissions</span></span>
<span data-ttu-id="fa61e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa61e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa61e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa61e-109">Permission type</span></span> |<span data-ttu-id="fa61e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa61e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="fa61e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa61e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa61e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa61e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="fa61e-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="fa61e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fa61e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa61e-114">Not supported.</span></span>|
|<span data-ttu-id="fa61e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa61e-115">Application</span></span>|<span data-ttu-id="fa61e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa61e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa61e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa61e-117">HTTP request</span></span>
```
POST /financials/companies/{id}/taxGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa61e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa61e-118">Optional query parameters</span></span>
<span data-ttu-id="fa61e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa61e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa61e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa61e-120">Request headers</span></span>

|<span data-ttu-id="fa61e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa61e-121">Header</span></span>|<span data-ttu-id="fa61e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fa61e-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="fa61e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa61e-123">Authorization</span></span>  |<span data-ttu-id="fa61e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa61e-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="fa61e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa61e-126">Content-Type</span></span>  |<span data-ttu-id="fa61e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fa61e-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="fa61e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa61e-128">Request body</span></span>
<span data-ttu-id="fa61e-129">No corpo da solicitação, forneça uma representação JSON de um objeto **taxGroups** .</span><span class="sxs-lookup"><span data-stu-id="fa61e-129">In the request body, supply a JSON representation of a **taxGroups** object.</span></span>

## <a name="response"></a><span data-ttu-id="fa61e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa61e-130">Response</span></span>
<span data-ttu-id="fa61e-131">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **taxGroups** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa61e-131">If successful, this method returns ```201 Created``` response code and a **taxGroups** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa61e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa61e-132">Example</span></span>

<span data-ttu-id="fa61e-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="fa61e-133">**Request**</span></span>

<span data-ttu-id="fa61e-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa61e-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxGroups
Content-type: application/json

{
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax"
}
```

<span data-ttu-id="fa61e-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="fa61e-135">**Response**</span></span>

<span data-ttu-id="fa61e-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa61e-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="fa61e-137">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa61e-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fa61e-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa61e-138">All the properties will be returned from an actual call.</span></span>

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
