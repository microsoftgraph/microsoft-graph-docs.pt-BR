---
title: Excluir moedas
description: Exclui um objeto Currency no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ce3980118a26276ab712e2c422b9260b8624b31c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956510"
---
# <a name="delete-currencies"></a><span data-ttu-id="2532f-103">Excluir moedas</span><span class="sxs-lookup"><span data-stu-id="2532f-103">Delete currencies</span></span>
<span data-ttu-id="2532f-104">Excluir um objeto Currency do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2532f-104">Delete a currency object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2532f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2532f-105">Permissions</span></span>
<span data-ttu-id="2532f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2532f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2532f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2532f-108">Permission type</span></span> |<span data-ttu-id="2532f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2532f-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2532f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2532f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2532f-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2532f-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2532f-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2532f-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2532f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2532f-113">Not supported.</span></span>|
|<span data-ttu-id="2532f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2532f-114">Application</span></span>|<span data-ttu-id="2532f-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2532f-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2532f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2532f-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/currencies('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2532f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2532f-117">Optional query parameters</span></span>
<span data-ttu-id="2532f-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2532f-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2532f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2532f-119">Request headers</span></span>

|<span data-ttu-id="2532f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2532f-120">Header</span></span>|<span data-ttu-id="2532f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2532f-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="2532f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2532f-122">Authorization</span></span>  |<span data-ttu-id="2532f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2532f-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="2532f-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="2532f-125">If-Match</span></span>       |<span data-ttu-id="2532f-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2532f-126">Required.</span></span> <span data-ttu-id="2532f-127">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas **moedas**, as **moedas** não serão</span><span class="sxs-lookup"><span data-stu-id="2532f-127">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be</span></span>
 <span data-ttu-id="2532f-128">atualizado.</span><span class="sxs-lookup"><span data-stu-id="2532f-128">updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2532f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2532f-129">Request body</span></span>
<span data-ttu-id="2532f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2532f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2532f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2532f-131">Response</span></span>
<span data-ttu-id="2532f-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2532f-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2532f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2532f-134">Example</span></span>

<span data-ttu-id="2532f-135">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="2532f-135">**Request**</span></span>

<span data-ttu-id="2532f-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2532f-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/currencies('{id}')
```

<span data-ttu-id="2532f-137">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="2532f-137">**Response**</span></span> 

<span data-ttu-id="2532f-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2532f-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
