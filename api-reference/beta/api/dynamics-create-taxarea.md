---
title: Criar taxAreas
description: Cria um objeto de área de impostos no Dynamics para finanças.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 7f2da2cc9540b1dc3d884fffe3a89fc50dbf32c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981605"
---
# <a name="create-taxareas"></a><span data-ttu-id="23e82-103">Criar taxAreas</span><span class="sxs-lookup"><span data-stu-id="23e82-103">Create taxAreas</span></span>

<span data-ttu-id="23e82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23e82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23e82-105">Cria um objeto de área de impostos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="23e82-105">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="23e82-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="23e82-106">Permissions</span></span>
<span data-ttu-id="23e82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23e82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23e82-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23e82-109">Permission type</span></span> |<span data-ttu-id="23e82-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23e82-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="23e82-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23e82-111">Delegated (work or school account)</span></span>|<span data-ttu-id="23e82-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e82-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="23e82-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="23e82-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="23e82-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23e82-114">Not supported.</span></span>|
|<span data-ttu-id="23e82-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23e82-115">Application</span></span>|<span data-ttu-id="23e82-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e82-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23e82-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23e82-117">HTTP request</span></span>

```
POST /financials/companies/{id}/taxAreas/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23e82-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23e82-118">Optional query parameters</span></span>
<span data-ttu-id="23e82-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23e82-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23e82-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23e82-120">Request headers</span></span>
|<span data-ttu-id="23e82-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23e82-121">Header</span></span>|<span data-ttu-id="23e82-122">Valor</span><span class="sxs-lookup"><span data-stu-id="23e82-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="23e82-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23e82-123">Authorization</span></span>  |<span data-ttu-id="23e82-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23e82-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="23e82-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23e82-126">Content-Type</span></span>  |<span data-ttu-id="23e82-127">application/json</span><span class="sxs-lookup"><span data-stu-id="23e82-127">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="23e82-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23e82-128">Request body</span></span>
<span data-ttu-id="23e82-129">No corpo da solicitação, forneça uma representação JSON de um objeto **taxAreas** .</span><span class="sxs-lookup"><span data-stu-id="23e82-129">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="23e82-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="23e82-130">Response</span></span>
<span data-ttu-id="23e82-131">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **taxAreas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23e82-131">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23e82-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23e82-132">Example</span></span>

<span data-ttu-id="23e82-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="23e82-133">**Request**</span></span>

<span data-ttu-id="23e82-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="23e82-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/taxAreas
Content-type: application/json

```json
{
  "code": "44442001T"
}
```

<span data-ttu-id="23e82-135">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="23e82-135">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "44442001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


