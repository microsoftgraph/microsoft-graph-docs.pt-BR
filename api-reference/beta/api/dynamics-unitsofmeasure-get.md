---
title: Obter unitsOfMeasure
description: Obtém um objeto de unidade de medida no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 7e8ff96f93d14659970bebd66f018e50aea3ab12
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42428142"
---
# <a name="get-unitsofmeasure"></a><span data-ttu-id="4d1a1-103">Obter unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="4d1a1-103">Get unitsOfMeasure</span></span>

<span data-ttu-id="4d1a1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4d1a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d1a1-105">Recupere as propriedades e os relacionamentos de um objeto de unidades de medida para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-105">Retrieve the properties and relationships of a units of measure object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d1a1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d1a1-106">Permissions</span></span>
<span data-ttu-id="4d1a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d1a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d1a1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d1a1-109">Permission type</span></span> |<span data-ttu-id="4d1a1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d1a1-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4d1a1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d1a1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d1a1-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d1a1-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4d1a1-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4d1a1-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4d1a1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-114">Not supported.</span></span>|
|<span data-ttu-id="4d1a1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d1a1-115">Application</span></span>|<span data-ttu-id="4d1a1-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d1a1-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d1a1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d1a1-117">HTTP request</span></span>

```
GET /financials/companies/{id}/unitsOfMeasure/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d1a1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4d1a1-118">Optional query parameters</span></span>
<span data-ttu-id="4d1a1-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d1a1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d1a1-120">Request headers</span></span>
|<span data-ttu-id="4d1a1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d1a1-121">Header</span></span>|<span data-ttu-id="4d1a1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4d1a1-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="4d1a1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d1a1-123">Authorization</span></span>  |<span data-ttu-id="4d1a1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d1a1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d1a1-126">Request body</span></span>
<span data-ttu-id="4d1a1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d1a1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d1a1-128">Response</span></span>
<span data-ttu-id="4d1a1-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **unitsOfMeasure** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-129">If successful, this method returns a `200 OK` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d1a1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d1a1-130">Example</span></span>

<span data-ttu-id="4d1a1-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="4d1a1-131">**Request**</span></span>

<span data-ttu-id="4d1a1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure/{id}
```

<span data-ttu-id="4d1a1-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="4d1a1-133">**Response**</span></span>

<span data-ttu-id="4d1a1-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="4d1a1-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4d1a1-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d1a1-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```
