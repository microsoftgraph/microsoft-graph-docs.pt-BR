---
title: Criar diários
description: Cria um objeto Journal no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6eae175fe8f9de73ba9db7d8b05bf4217d7a9a36
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956636"
---
# <a name="create-journals"></a><span data-ttu-id="c5cc5-103">Criar diários</span><span class="sxs-lookup"><span data-stu-id="c5cc5-103">Create journals</span></span>
<span data-ttu-id="c5cc5-104">Cria um diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="c5cc5-104">Creates a journal in Dynamics 365 Business Central.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c5cc5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5cc5-105">Permissions</span></span>
<span data-ttu-id="c5cc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5cc5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5cc5-108">Permission type</span></span> |<span data-ttu-id="c5cc5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5cc5-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c5cc5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5cc5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c5cc5-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5cc5-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c5cc5-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="c5cc5-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c5cc5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5cc5-113">Not supported.</span></span>|
|<span data-ttu-id="c5cc5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5cc5-114">Application</span></span>|<span data-ttu-id="c5cc5-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5cc5-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5cc5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5cc5-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/journals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5cc5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5cc5-117">Optional query parameters</span></span>
<span data-ttu-id="c5cc5-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5cc5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5cc5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5cc5-119">Request headers</span></span>
|<span data-ttu-id="c5cc5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5cc5-120">Header</span></span>        |<span data-ttu-id="c5cc5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c5cc5-121">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="c5cc5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5cc5-122">Authorization</span></span> |<span data-ttu-id="c5cc5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5cc5-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c5cc5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5cc5-125">Content-Type</span></span>  |<span data-ttu-id="c5cc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5cc5-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="c5cc5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5cc5-127">Request body</span></span>
<span data-ttu-id="c5cc5-128">No corpo da solicitação, forneça uma representação JSON de um \*\*\*\* objeto Journals.</span><span class="sxs-lookup"><span data-stu-id="c5cc5-128">In the request body, supply a JSON representation of a **journals** object.</span></span>

## <a name="response"></a><span data-ttu-id="c5cc5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5cc5-129">Response</span></span>
<span data-ttu-id="c5cc5-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **Journals** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5cc5-130">If successful, this method returns ```201 Created``` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5cc5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5cc5-131">Example</span></span>

<span data-ttu-id="c5cc5-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c5cc5-132">**Request**</span></span>

<span data-ttu-id="c5cc5-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5cc5-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/journals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="c5cc5-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="c5cc5-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

