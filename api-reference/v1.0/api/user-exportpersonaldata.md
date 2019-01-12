---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar dados de um usuário organizacionais.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba26d2b2bc5af63f01a4333490d9850ffa3dd767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954299"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="d5495-103">usuário: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="d5495-103">user: exportPersonalData</span></span>

<span data-ttu-id="d5495-104">Envie uma solicitação de operação de política de dados de um administrador da empresa ou de um aplicativo para exportar dados de um usuário organizacional.</span><span class="sxs-lookup"><span data-stu-id="d5495-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5495-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5495-105">Permissions</span></span>
<span data-ttu-id="d5495-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5495-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5495-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5495-108">Permission type</span></span>      | <span data-ttu-id="d5495-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5495-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5495-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5495-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d5495-111">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5495-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="d5495-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5495-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d5495-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="d5495-113">Not applicable</span></span>  |
|<span data-ttu-id="d5495-114">Aplicação</span><span class="sxs-lookup"><span data-stu-id="d5495-114">Application</span></span> | <span data-ttu-id="d5495-115">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5495-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="d5495-116">**Observação:** A exportação só pode ser executada por um administrador da empresa quando permissões delegadas são usadas.</span><span class="sxs-lookup"><span data-stu-id="d5495-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="d5495-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5495-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="d5495-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5495-118">Request headers</span></span>
| <span data-ttu-id="d5495-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d5495-119">Name</span></span>       | <span data-ttu-id="d5495-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5495-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5495-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5495-121">Authorization</span></span>  | <span data-ttu-id="d5495-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d5495-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5495-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5495-123">Request body</span></span>
<span data-ttu-id="d5495-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5495-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d5495-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5495-125">Parameter</span></span>    | <span data-ttu-id="d5495-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5495-126">Type</span></span>   |<span data-ttu-id="d5495-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5495-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5495-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="d5495-128">storageLocation</span></span>|<span data-ttu-id="d5495-129">String</span><span class="sxs-lookup"><span data-stu-id="d5495-129">String</span></span>|<span data-ttu-id="d5495-130">Esta é uma URL de assinatura (SAS) de acesso compartilhado para uma conta de armazenamento do Azure, para onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="d5495-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="d5495-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5495-131">Response</span></span>
<span data-ttu-id="d5495-132">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d5495-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="d5495-133">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5495-133">It does not return anything in the response body.</span></span> <span data-ttu-id="d5495-134">A resposta conterá os seguintes cabeçalhos de resposta.</span><span class="sxs-lookup"><span data-stu-id="d5495-134">The response contains the following response headers.</span></span>

| <span data-ttu-id="d5495-135">Nome</span><span class="sxs-lookup"><span data-stu-id="d5495-135">Name</span></span>       | <span data-ttu-id="d5495-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5495-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5495-137">Location</span><span class="sxs-lookup"><span data-stu-id="d5495-137">Location</span></span>  | <span data-ttu-id="d5495-138">URL para verificar o status da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5495-138">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="d5495-139">Depois de repetição</span><span class="sxs-lookup"><span data-stu-id="d5495-139">Retry-After</span></span>  | <span data-ttu-id="d5495-140">Período de tempo em segundos.</span><span class="sxs-lookup"><span data-stu-id="d5495-140">Time period in seconds.</span></span> <span data-ttu-id="d5495-141">Criador de solicitação deve aguardar esta tempo depois de enviar uma solicitação para verificar o status.</span><span class="sxs-lookup"><span data-stu-id="d5495-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="d5495-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5495-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5495-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5495-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a><span data-ttu-id="d5495-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5495-144">Response</span></span>

```
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
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
