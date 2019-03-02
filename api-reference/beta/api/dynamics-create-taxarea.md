---
title: Criar taxAreas
description: Cria um objeto de área de impostos no Dynamics para finanças.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6addfb3617b05bcb8b6a12d6df31e115d5ea01a9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365763"
---
# <a name="create-taxareas"></a><span data-ttu-id="28257-103">Criar taxAreas</span><span class="sxs-lookup"><span data-stu-id="28257-103">Create taxAreas</span></span>
<span data-ttu-id="28257-104">Cria um objeto de área de impostos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="28257-104">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="28257-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="28257-105">Permissions</span></span>
<span data-ttu-id="28257-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28257-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28257-108">Permission type</span></span> |<span data-ttu-id="28257-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28257-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="28257-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28257-110">Delegated (work or school account)</span></span>|<span data-ttu-id="28257-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28257-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="28257-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="28257-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="28257-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28257-113">Not supported.</span></span>|
|<span data-ttu-id="28257-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28257-114">Application</span></span>|<span data-ttu-id="28257-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28257-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28257-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28257-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/taxAreas('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28257-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28257-117">Optional query parameters</span></span>
<span data-ttu-id="28257-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28257-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28257-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28257-119">Request headers</span></span>
|<span data-ttu-id="28257-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28257-120">Header</span></span>|<span data-ttu-id="28257-121">Valor</span><span class="sxs-lookup"><span data-stu-id="28257-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="28257-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="28257-122">Authorization</span></span>  |<span data-ttu-id="28257-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28257-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="28257-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28257-125">Content-Type</span></span>  |<span data-ttu-id="28257-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28257-126">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="28257-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28257-127">Request body</span></span>
<span data-ttu-id="28257-128">No corpo da solicitação, forneça uma representação JSON de um objeto **taxAreas** .</span><span class="sxs-lookup"><span data-stu-id="28257-128">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="28257-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="28257-129">Response</span></span>
<span data-ttu-id="28257-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **taxAreas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28257-130">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28257-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28257-131">Example</span></span>

<span data-ttu-id="28257-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="28257-132">**Request**</span></span>

<span data-ttu-id="28257-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="28257-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/taxAreas
Content-type: application/json

```json
{
  "code": "44442001T"
}
```

<span data-ttu-id="28257-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="28257-134">**Response**</span></span>

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
