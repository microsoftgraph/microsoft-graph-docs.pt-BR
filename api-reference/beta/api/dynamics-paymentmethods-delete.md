---
title: Excluir paymentMethods
description: Exclui um objeto de método de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7b418160573eb9acf2f0c9e9f2ab0d352b59d846
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366603"
---
# <a name="delete-paymentmethods"></a><span data-ttu-id="12df1-103">Excluir paymentMethods</span><span class="sxs-lookup"><span data-stu-id="12df1-103">Delete paymentMethods</span></span>
<span data-ttu-id="12df1-104">Excluir um objeto de método de pagamento do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="12df1-104">Delete a payment method object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="12df1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="12df1-105">Permissions</span></span>
<span data-ttu-id="12df1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12df1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12df1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12df1-108">Permission type</span></span> |<span data-ttu-id="12df1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12df1-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="12df1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12df1-110">Delegated (work or school account)</span></span>|<span data-ttu-id="12df1-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12df1-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="12df1-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="12df1-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="12df1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12df1-113">Not supported.</span></span>|
|<span data-ttu-id="12df1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12df1-114">Application</span></span>|<span data-ttu-id="12df1-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12df1-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12df1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12df1-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/paymentMethods('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12df1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12df1-117">Optional query parameters</span></span>
<span data-ttu-id="12df1-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12df1-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12df1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12df1-119">Request headers</span></span>

|<span data-ttu-id="12df1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12df1-120">Header</span></span>         |<span data-ttu-id="12df1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="12df1-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="12df1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12df1-122">Authorization</span></span>  |<span data-ttu-id="12df1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12df1-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="12df1-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="12df1-125">If-Match</span></span>       |<span data-ttu-id="12df1-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12df1-126">Required.</span></span> <span data-ttu-id="12df1-127">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **paymentMethods**, o **paymentMethods** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="12df1-127">When this request header is included and the eTag provided does not match the current tag on the **paymentMethods**, the **paymentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12df1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12df1-128">Request body</span></span>
<span data-ttu-id="12df1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12df1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12df1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="12df1-130">Response</span></span>
<span data-ttu-id="12df1-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12df1-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12df1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12df1-133">Example</span></span>

<span data-ttu-id="12df1-134">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="12df1-134">**Request**</span></span>

<span data-ttu-id="12df1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12df1-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/paymentMethods('{id}')
```

<span data-ttu-id="12df1-136">**Response**</span><span class="sxs-lookup"><span data-stu-id="12df1-136">**Response**</span></span> 

<span data-ttu-id="12df1-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12df1-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```

