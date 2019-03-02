---
title: Excluir customerPaymentJournals
description: Exclui um diário de pagamento do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6309aac868d360867e4690e6efa71ebd64a5fbb3
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365546"
---
# <a name="delete-customerpaymentjournals"></a><span data-ttu-id="a54c7-103">Excluir customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="a54c7-103">Delete customerPaymentJournals</span></span>
<span data-ttu-id="a54c7-104">Excluir um objeto de diário de pagamento de cliente do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="a54c7-104">Delete a customer payment journal object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a54c7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a54c7-105">Permissions</span></span>
<span data-ttu-id="a54c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a54c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a54c7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a54c7-108">Permission type</span></span> |<span data-ttu-id="a54c7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a54c7-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a54c7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a54c7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="a54c7-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a54c7-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a54c7-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a54c7-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a54c7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a54c7-113">Not supported.</span></span>|
|<span data-ttu-id="a54c7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a54c7-114">Application</span></span>|<span data-ttu-id="a54c7-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a54c7-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a54c7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a54c7-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/customerPaymentJournals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a54c7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a54c7-117">Optional query parameters</span></span>
<span data-ttu-id="a54c7-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a54c7-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a54c7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a54c7-119">Request headers</span></span>
|<span data-ttu-id="a54c7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a54c7-120">Header</span></span>       |<span data-ttu-id="a54c7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a54c7-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="a54c7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a54c7-122">Authorization</span></span>|<span data-ttu-id="a54c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a54c7-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="a54c7-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="a54c7-125">If-Match</span></span>     |<span data-ttu-id="a54c7-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a54c7-126">Required.</span></span> <span data-ttu-id="a54c7-127">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **customerPaymentJournals**, o **customerPaymentJournals** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="a54c7-127">When this request header is included and the eTag provided does not match the current tag on the **customerPaymentJournals**, the **customerPaymentJournals** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a54c7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a54c7-128">Request body</span></span>

<span data-ttu-id="a54c7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a54c7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a54c7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a54c7-130">Response</span></span>

<span data-ttu-id="a54c7-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a54c7-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a54c7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a54c7-133">Example</span></span>

<span data-ttu-id="a54c7-134">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="a54c7-134">**Request**</span></span>

<span data-ttu-id="a54c7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a54c7-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals('{id}')
```

<span data-ttu-id="a54c7-136">**Response**</span><span class="sxs-lookup"><span data-stu-id="a54c7-136">**Response**</span></span> 

<span data-ttu-id="a54c7-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a54c7-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```

