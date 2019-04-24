---
title: Obter shipmentMethods
description: Obtém um objeto de método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 3391b6a492ea0edad51c49712290ca88f4535106
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458513"
---
# <a name="get-shipmentmethods"></a><span data-ttu-id="36095-103">Obter shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="36095-103">Get shipmentMethods</span></span>
<span data-ttu-id="36095-104">Recupere as propriedades e os relacionamentos de um objeto de método de remessa para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="36095-104">Retrieve the properties and relationships of a shipment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="36095-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="36095-105">Permissions</span></span>
<span data-ttu-id="36095-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36095-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36095-108">Permission type</span></span> |<span data-ttu-id="36095-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36095-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="36095-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36095-110">Delegated (work or school account)</span></span>|<span data-ttu-id="36095-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36095-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="36095-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="36095-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="36095-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36095-113">Not supported.</span></span>|
|<span data-ttu-id="36095-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36095-114">Application</span></span>|<span data-ttu-id="36095-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36095-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36095-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36095-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/shipmentMethods('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36095-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36095-117">Optional query parameters</span></span>
<span data-ttu-id="36095-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36095-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36095-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36095-119">Request headers</span></span>
|<span data-ttu-id="36095-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36095-120">Header</span></span>|<span data-ttu-id="36095-121">Valor</span><span class="sxs-lookup"><span data-stu-id="36095-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="36095-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="36095-122">Authorization</span></span>  |<span data-ttu-id="36095-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36095-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36095-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36095-125">Request body</span></span>
<span data-ttu-id="36095-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36095-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36095-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="36095-127">Response</span></span>
<span data-ttu-id="36095-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **shipmentMethods** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36095-128">If successful, this method returns a `200 OK` response code and a **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36095-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36095-129">Example</span></span>

<span data-ttu-id="36095-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="36095-130">**Request**</span></span>

<span data-ttu-id="36095-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36095-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/shipmentMethods('{id}')
```

<span data-ttu-id="36095-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="36095-132">**Response**</span></span>

<span data-ttu-id="36095-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36095-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="36095-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36095-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="36095-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36095-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}
```

