---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar os dados de um usuário organizacional.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f112d065b75da7dc525e667df78b0264be37d55
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547897"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="e5bee-103">usuário: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="e5bee-103">user: exportPersonalData</span></span>

<span data-ttu-id="e5bee-104">Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar os dados de um usuário organizacional.</span><span class="sxs-lookup"><span data-stu-id="e5bee-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5bee-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5bee-105">Permissions</span></span>
<span data-ttu-id="e5bee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5bee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5bee-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5bee-108">Permission type</span></span>      | <span data-ttu-id="e5bee-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5bee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5bee-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5bee-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5bee-111">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="e5bee-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="e5bee-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5bee-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e5bee-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="e5bee-113">Not applicable</span></span>  |
|<span data-ttu-id="e5bee-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5bee-114">Application</span></span> | <span data-ttu-id="e5bee-115">User. Export. All e User. Read. All</span><span class="sxs-lookup"><span data-stu-id="e5bee-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="e5bee-116">**Observação:** A exportação só pode ser realizada por um administrador da empresa quando a permissão delegada é usada.</span><span class="sxs-lookup"><span data-stu-id="e5bee-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="e5bee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5bee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="e5bee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5bee-118">Request headers</span></span>
| <span data-ttu-id="e5bee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e5bee-119">Name</span></span>       | <span data-ttu-id="e5bee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5bee-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e5bee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5bee-121">Authorization</span></span>  | <span data-ttu-id="e5bee-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e5bee-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5bee-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5bee-123">Request body</span></span>
<span data-ttu-id="e5bee-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5bee-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e5bee-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e5bee-125">Parameter</span></span>    | <span data-ttu-id="e5bee-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5bee-126">Type</span></span>   |<span data-ttu-id="e5bee-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5bee-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e5bee-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="e5bee-128">storageLocation</span></span>|<span data-ttu-id="e5bee-129">String</span><span class="sxs-lookup"><span data-stu-id="e5bee-129">String</span></span>|<span data-ttu-id="e5bee-130">Esta é uma URL de assinatura de acesso compartilhado (SAS) para uma conta de armazenamento do Azure, onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="e5bee-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="e5bee-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5bee-131">Response</span></span>
<span data-ttu-id="e5bee-132">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="e5bee-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="e5bee-133">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5bee-133">It does not return anything in the response body.</span></span> <span data-ttu-id="e5bee-134">A resposta contém os cabeçalhos a seguir.</span><span class="sxs-lookup"><span data-stu-id="e5bee-134">The response contains the following headers.</span></span>

| <span data-ttu-id="e5bee-135">Nome</span><span class="sxs-lookup"><span data-stu-id="e5bee-135">Name</span></span>       | <span data-ttu-id="e5bee-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5bee-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e5bee-137">Local</span><span class="sxs-lookup"><span data-stu-id="e5bee-137">Location</span></span>  | <span data-ttu-id="e5bee-138">URL para verificar o status da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5bee-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="e5bee-139">Repetir-após</span><span class="sxs-lookup"><span data-stu-id="e5bee-139">Retry-After</span></span>  | <span data-ttu-id="e5bee-140">Período de tempo em segundos.</span><span class="sxs-lookup"><span data-stu-id="e5bee-140">Time period in seconds.</span></span> <span data-ttu-id="e5bee-141">O criador de solicitação deve aguardar esse tempo depois de enviar uma solicitação para verificar o status.</span><span class="sxs-lookup"><span data-stu-id="e5bee-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="e5bee-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5bee-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5bee-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5bee-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a><span data-ttu-id="e5bee-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5bee-144">Response</span></span>

```
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
