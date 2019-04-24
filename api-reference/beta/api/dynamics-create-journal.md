---
title: Criar diários
description: Cria um objeto Journal no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 27bef92d9392cd6369564e86417b438ed8bd5a5a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463632"
---
# <a name="create-journals"></a><span data-ttu-id="e7bbd-103">Criar diários</span><span class="sxs-lookup"><span data-stu-id="e7bbd-103">Create journals</span></span>
<span data-ttu-id="e7bbd-104">Cria um diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="e7bbd-104">Creates a journal in Dynamics 365 Business Central.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e7bbd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7bbd-105">Permissions</span></span>
<span data-ttu-id="e7bbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7bbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7bbd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7bbd-108">Permission type</span></span> |<span data-ttu-id="e7bbd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7bbd-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e7bbd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7bbd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e7bbd-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7bbd-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e7bbd-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e7bbd-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e7bbd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7bbd-113">Not supported.</span></span>|
|<span data-ttu-id="e7bbd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7bbd-114">Application</span></span>|<span data-ttu-id="e7bbd-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7bbd-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7bbd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7bbd-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/journals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7bbd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7bbd-117">Optional query parameters</span></span>
<span data-ttu-id="e7bbd-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7bbd-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7bbd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7bbd-119">Request headers</span></span>
|<span data-ttu-id="e7bbd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7bbd-120">Header</span></span>        |<span data-ttu-id="e7bbd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7bbd-121">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="e7bbd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7bbd-122">Authorization</span></span> |<span data-ttu-id="e7bbd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7bbd-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e7bbd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7bbd-125">Content-Type</span></span>  |<span data-ttu-id="e7bbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7bbd-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="e7bbd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7bbd-127">Request body</span></span>
<span data-ttu-id="e7bbd-128">No corpo da solicitação, forneça uma representação JSON de um \*\*\*\* objeto Journals.</span><span class="sxs-lookup"><span data-stu-id="e7bbd-128">In the request body, supply a JSON representation of a **journals** object.</span></span>

## <a name="response"></a><span data-ttu-id="e7bbd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7bbd-129">Response</span></span>
<span data-ttu-id="e7bbd-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **Journals** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7bbd-130">If successful, this method returns ```201 Created``` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7bbd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7bbd-131">Example</span></span>

<span data-ttu-id="e7bbd-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="e7bbd-132">**Request**</span></span>

<span data-ttu-id="e7bbd-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7bbd-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/journals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="e7bbd-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="e7bbd-134">**Response**</span></span>

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

