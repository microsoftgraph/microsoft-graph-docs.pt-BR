---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar dados de um usuário organizacionais.
ms.openlocfilehash: ffde9af132fbb15706fe54af8a6b3aaeba07d12b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748266"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="26ddb-103">usuário: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="26ddb-103">user: exportPersonalData</span></span>

<span data-ttu-id="26ddb-104">Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar dados de um usuário organizacionais.</span><span class="sxs-lookup"><span data-stu-id="26ddb-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="26ddb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="26ddb-105">Permissions</span></span>
<span data-ttu-id="26ddb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26ddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26ddb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26ddb-108">Permission type</span></span>      | <span data-ttu-id="26ddb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26ddb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26ddb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26ddb-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="26ddb-111">User.Export.All e User.Read.All</span><span class="sxs-lookup"><span data-stu-id="26ddb-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="26ddb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26ddb-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="26ddb-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="26ddb-113">Not applicable</span></span>  |
|<span data-ttu-id="26ddb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26ddb-114">Application</span></span> | <span data-ttu-id="26ddb-115">User.Export.All e User.Read.All</span><span class="sxs-lookup"><span data-stu-id="26ddb-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="26ddb-116">**Observação:** Exportação só pode ser executada por um administrador da empresa, quando a permissão delegada é usada.</span><span class="sxs-lookup"><span data-stu-id="26ddb-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="26ddb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26ddb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="26ddb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26ddb-118">Request headers</span></span>
| <span data-ttu-id="26ddb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26ddb-119">Name</span></span>       | <span data-ttu-id="26ddb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ddb-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="26ddb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="26ddb-121">Authorization</span></span>  | <span data-ttu-id="26ddb-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="26ddb-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="26ddb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26ddb-123">Request body</span></span>
<span data-ttu-id="26ddb-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26ddb-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="26ddb-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="26ddb-125">Parameter</span></span>    | <span data-ttu-id="26ddb-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="26ddb-126">Type</span></span>   |<span data-ttu-id="26ddb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ddb-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="26ddb-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="26ddb-128">storageLocation</span></span>|<span data-ttu-id="26ddb-129">String</span><span class="sxs-lookup"><span data-stu-id="26ddb-129">String</span></span>|<span data-ttu-id="26ddb-130">Esta é uma URL de assinatura (SAS) de acesso compartilhado para uma conta de armazenamento do Azure, para onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="26ddb-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="26ddb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ddb-131">Response</span></span>
<span data-ttu-id="26ddb-132">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="26ddb-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="26ddb-133">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26ddb-133">It does not return anything in the response body.</span></span> <span data-ttu-id="26ddb-134">A resposta conterá os seguintes cabeçalhos.</span><span class="sxs-lookup"><span data-stu-id="26ddb-134">The response contains the following headers.</span></span>

| <span data-ttu-id="26ddb-135">Nome</span><span class="sxs-lookup"><span data-stu-id="26ddb-135">Name</span></span>       | <span data-ttu-id="26ddb-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ddb-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="26ddb-137">Location</span><span class="sxs-lookup"><span data-stu-id="26ddb-137">Location</span></span>  | <span data-ttu-id="26ddb-138">URL para verificar o status da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26ddb-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="26ddb-139">Depois de repetição</span><span class="sxs-lookup"><span data-stu-id="26ddb-139">Retry-After</span></span>  | <span data-ttu-id="26ddb-140">Período de tempo em segundos.</span><span class="sxs-lookup"><span data-stu-id="26ddb-140">Time period in seconds.</span></span> <span data-ttu-id="26ddb-141">Criador de solicitação deve aguardar esta tempo depois de enviar uma solicitação para verificar o status.</span><span class="sxs-lookup"><span data-stu-id="26ddb-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="26ddb-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26ddb-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26ddb-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26ddb-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="26ddb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ddb-144">Response</span></span>

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
