---
title: Obter taxAreas
description: Obtém um objeto de área de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 50c119a08e547d87afa2eeb40e790b5e98e7b68d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791250"
---
# <a name="get-taxareas"></a><span data-ttu-id="0013a-103">Obter taxAreas</span><span class="sxs-lookup"><span data-stu-id="0013a-103">Get taxAreas</span></span>
<span data-ttu-id="0013a-104">Recupere as propriedades e os relacionamentos de um objeto de área de impostos para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="0013a-104">Retrieve the properties and relationships of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="0013a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0013a-105">Permissions</span></span>
<span data-ttu-id="0013a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0013a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0013a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0013a-108">Permission type</span></span> |<span data-ttu-id="0013a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0013a-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="0013a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0013a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0013a-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0013a-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="0013a-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="0013a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0013a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0013a-113">Not supported.</span></span>|
|<span data-ttu-id="0013a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0013a-114">Application</span></span>|<span data-ttu-id="0013a-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0013a-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0013a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0013a-116">HTTP request</span></span>

```
GET /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0013a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0013a-117">Optional query parameters</span></span>
<span data-ttu-id="0013a-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0013a-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0013a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0013a-119">Request headers</span></span>
|<span data-ttu-id="0013a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0013a-120">Header</span></span>|<span data-ttu-id="0013a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0013a-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="0013a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0013a-122">Authorization</span></span>  |<span data-ttu-id="0013a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0013a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0013a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0013a-125">Request body</span></span>
<span data-ttu-id="0013a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0013a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0013a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0013a-127">Response</span></span>
<span data-ttu-id="0013a-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **taxAreas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0013a-128">If successful, this method returns a `200 OK` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0013a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0013a-129">Example</span></span>

<span data-ttu-id="0013a-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="0013a-130">**Request**</span></span>

<span data-ttu-id="0013a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0013a-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas/{id}
```

<span data-ttu-id="0013a-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="0013a-132">**Response**</span></span>

<span data-ttu-id="0013a-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0013a-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="0013a-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0013a-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0013a-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0013a-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

