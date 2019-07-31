---
title: Criar taxGroups
description: Cria um objeto de grupo de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 31d4907248d64a5200e1dbae9e4b2626f46b2ee1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956552"
---
# <a name="create-taxgroups"></a><span data-ttu-id="afe88-103">Criar taxGroups</span><span class="sxs-lookup"><span data-stu-id="afe88-103">Create taxGroups</span></span>
<span data-ttu-id="afe88-104">Criar um objeto de grupos de impostos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="afe88-104">Create a tax groups object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="afe88-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="afe88-105">Permissions</span></span>
<span data-ttu-id="afe88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afe88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe88-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afe88-108">Permission type</span></span> |<span data-ttu-id="afe88-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="afe88-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="afe88-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afe88-110">Delegated (work or school account)</span></span>|<span data-ttu-id="afe88-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe88-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="afe88-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="afe88-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="afe88-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afe88-113">Not supported.</span></span>|
|<span data-ttu-id="afe88-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afe88-114">Application</span></span>|<span data-ttu-id="afe88-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe88-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afe88-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afe88-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/taxGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afe88-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="afe88-117">Optional query parameters</span></span>
<span data-ttu-id="afe88-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="afe88-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afe88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afe88-119">Request headers</span></span>

|<span data-ttu-id="afe88-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afe88-120">Header</span></span>|<span data-ttu-id="afe88-121">Valor</span><span class="sxs-lookup"><span data-stu-id="afe88-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="afe88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="afe88-122">Authorization</span></span>  |<span data-ttu-id="afe88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afe88-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="afe88-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afe88-125">Content-Type</span></span>  |<span data-ttu-id="afe88-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afe88-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="afe88-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afe88-127">Request body</span></span>
<span data-ttu-id="afe88-128">No corpo da solicitação, forneça uma representação JSON de um objeto **taxGroups** .</span><span class="sxs-lookup"><span data-stu-id="afe88-128">In the request body, supply a JSON representation of a **taxGroups** object.</span></span>

## <a name="response"></a><span data-ttu-id="afe88-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="afe88-129">Response</span></span>
<span data-ttu-id="afe88-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **taxGroups** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afe88-130">If successful, this method returns ```201 Created``` response code and a **taxGroups** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afe88-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afe88-131">Example</span></span>

<span data-ttu-id="afe88-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="afe88-132">**Request**</span></span>

<span data-ttu-id="afe88-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="afe88-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/taxGroups
Content-type: application/json

{
  "code": "FURNITURE",
  "displayName": "Taxable Olympic Furniture",
  "taxType": "Sales Tax"
}
```

<span data-ttu-id="afe88-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="afe88-134">**Response**</span></span>

<span data-ttu-id="afe88-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afe88-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="afe88-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="afe88-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="afe88-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afe88-137">All the properties will be returned from an actual call.</span></span>

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
