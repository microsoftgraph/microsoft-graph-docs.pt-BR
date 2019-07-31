---
title: Obter unitsOfMeasure
description: Obtém um objeto de unidade de medida no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 89db4f4b3a1178c3de56c34340d00edbf8efb6e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955852"
---
# <a name="get-unitsofmeasure"></a><span data-ttu-id="7e2e7-103">Obter unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="7e2e7-103">Get unitsOfMeasure</span></span>
<span data-ttu-id="7e2e7-104">Recupere as propriedades e os relacionamentos de um objeto de unidades de medida para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-104">Retrieve the properties and relationships of a units of measure object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e2e7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e2e7-105">Permissions</span></span>
<span data-ttu-id="7e2e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e2e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e2e7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e2e7-108">Permission type</span></span> |<span data-ttu-id="7e2e7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e2e7-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7e2e7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e2e7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7e2e7-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2e7-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7e2e7-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="7e2e7-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7e2e7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-113">Not supported.</span></span>|
|<span data-ttu-id="7e2e7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e2e7-114">Application</span></span>|<span data-ttu-id="7e2e7-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2e7-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e2e7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e2e7-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/unitsOfMeasure('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e2e7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e2e7-117">Optional query parameters</span></span>
<span data-ttu-id="7e2e7-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e2e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e2e7-119">Request headers</span></span>
|<span data-ttu-id="7e2e7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e2e7-120">Header</span></span>|<span data-ttu-id="7e2e7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7e2e7-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="7e2e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e2e7-122">Authorization</span></span>  |<span data-ttu-id="7e2e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e2e7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e2e7-125">Request body</span></span>
<span data-ttu-id="7e2e7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e2e7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e2e7-127">Response</span></span>
<span data-ttu-id="7e2e7-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **unitsOfMeasure** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-128">If successful, this method returns a `200 OK` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e2e7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e2e7-129">Example</span></span>

<span data-ttu-id="7e2e7-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="7e2e7-130">**Request**</span></span>

<span data-ttu-id="7e2e7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/unitsOfMeasure('{id}')
```

<span data-ttu-id="7e2e7-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="7e2e7-132">**Response**</span></span>

<span data-ttu-id="7e2e7-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="7e2e7-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7e2e7-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e2e7-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```
