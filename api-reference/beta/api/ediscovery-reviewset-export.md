---
title: 'reviewSet: export'
description: Inicie uma exportação de um reviewSet.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7ee3744470cf5fac31abad2d4cc53ba47a0feca5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445777"
---
# <a name="reviewset-export"></a><span data-ttu-id="457ca-103">reviewSet: export</span><span class="sxs-lookup"><span data-stu-id="457ca-103">reviewSet: export</span></span>

<span data-ttu-id="457ca-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="457ca-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="457ca-105">Iniciar uma exportação de um **reviewSet**.</span><span class="sxs-lookup"><span data-stu-id="457ca-105">Initiate an export from a **reviewSet**.</span></span>  <span data-ttu-id="457ca-106">Para obter detalhes, [consulte Export documents from a review set in Advanced eDiscovery](/microsoft-365/compliance/export-documents-from-review-set).</span><span class="sxs-lookup"><span data-stu-id="457ca-106">For details, see [Export documents from a review set in Advanced eDiscovery](/microsoft-365/compliance/export-documents-from-review-set).</span></span>

## <a name="permissions"></a><span data-ttu-id="457ca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="457ca-107">Permissions</span></span>

<span data-ttu-id="457ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="457ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="457ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="457ca-110">Permission type</span></span>|<span data-ttu-id="457ca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="457ca-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="457ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="457ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="457ca-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457ca-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="457ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="457ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="457ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="457ca-115">Not supported.</span></span>|
|<span data-ttu-id="457ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="457ca-116">Application</span></span>|<span data-ttu-id="457ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="457ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="457ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="457ca-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewsets/{reviewsetId}/export
```

## <a name="request-headers"></a><span data-ttu-id="457ca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="457ca-119">Request headers</span></span>

|<span data-ttu-id="457ca-120">Nome</span><span class="sxs-lookup"><span data-stu-id="457ca-120">Name</span></span>|<span data-ttu-id="457ca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="457ca-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="457ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="457ca-122">Authorization</span></span>|<span data-ttu-id="457ca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="457ca-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="457ca-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="457ca-125">Content-Type</span></span>|<span data-ttu-id="457ca-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="457ca-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="457ca-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="457ca-128">Request body</span></span>

<span data-ttu-id="457ca-129">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="457ca-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="457ca-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="457ca-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="457ca-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="457ca-131">Parameter</span></span>|<span data-ttu-id="457ca-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="457ca-132">Type</span></span>|<span data-ttu-id="457ca-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="457ca-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457ca-134">outputName</span><span class="sxs-lookup"><span data-stu-id="457ca-134">outputName</span></span>|<span data-ttu-id="457ca-135">String</span><span class="sxs-lookup"><span data-stu-id="457ca-135">String</span></span>| <span data-ttu-id="457ca-136">Nome da exportação.</span><span class="sxs-lookup"><span data-stu-id="457ca-136">Name of the export.</span></span> <span data-ttu-id="457ca-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="457ca-137">Required.</span></span> |
|<span data-ttu-id="457ca-138">description</span><span class="sxs-lookup"><span data-stu-id="457ca-138">description</span></span>|<span data-ttu-id="457ca-139">String</span><span class="sxs-lookup"><span data-stu-id="457ca-139">String</span></span>| <span data-ttu-id="457ca-140">Descrição da exportação</span><span class="sxs-lookup"><span data-stu-id="457ca-140">Description of the export</span></span> |
|<span data-ttu-id="457ca-141">azureBlobContainer</span><span class="sxs-lookup"><span data-stu-id="457ca-141">azureBlobContainer</span></span>|<span data-ttu-id="457ca-142">String</span><span class="sxs-lookup"><span data-stu-id="457ca-142">String</span></span>| <span data-ttu-id="457ca-143">Ao exportar para sua própria conta de armazenamento do Azure, essa é a URL do contêiner.</span><span class="sxs-lookup"><span data-stu-id="457ca-143">When exporting to your own Azure storage account, this is the container URL.</span></span> |
|<span data-ttu-id="457ca-144">azureBlobToken</span><span class="sxs-lookup"><span data-stu-id="457ca-144">azureBlobToken</span></span>|<span data-ttu-id="457ca-145">String</span><span class="sxs-lookup"><span data-stu-id="457ca-145">String</span></span>| <span data-ttu-id="457ca-146">Ao exportar para sua própria conta de armazenamento do Azure, o token SAS para a URL do contêiner.</span><span class="sxs-lookup"><span data-stu-id="457ca-146">When exporting to your own Azure storage account, SAS token for the container URL.</span></span> |
|<span data-ttu-id="457ca-147">exportOptions</span><span class="sxs-lookup"><span data-stu-id="457ca-147">exportOptions</span></span>| [<span data-ttu-id="457ca-148">microsoft.graph.ediscovery.exportOptions</span><span class="sxs-lookup"><span data-stu-id="457ca-148">microsoft.graph.ediscovery.exportOptions</span></span>](../resources/ediscovery-caseexportoperation.md#exportoptions-values) |<span data-ttu-id="457ca-149">Especifica opções que controlam o formato da exportação.</span><span class="sxs-lookup"><span data-stu-id="457ca-149">Specifies options that control the format of the export.</span></span> <span data-ttu-id="457ca-150">Os valores possíveis são: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span><span class="sxs-lookup"><span data-stu-id="457ca-150">Possible values are: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span></span>|
|<span data-ttu-id="457ca-151">exportStructure</span><span class="sxs-lookup"><span data-stu-id="457ca-151">exportStructure</span></span>|[<span data-ttu-id="457ca-152">microsoft.graph.ediscovery.exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="457ca-152">microsoft.graph.ediscovery.exportFileStructure</span></span>](../resources/ediscovery-caseexportoperation.md#exportfilestructure-values)| <span data-ttu-id="457ca-153">Opções que controlam a estrutura do arquivo e o empacotamento da exportação.</span><span class="sxs-lookup"><span data-stu-id="457ca-153">Options that control file structure and packaging of the export.</span></span> <span data-ttu-id="457ca-154">Os valores possíveis são: `none`, `directory`, `pst`.</span><span class="sxs-lookup"><span data-stu-id="457ca-154">Possible values are: `none`, `directory`, `pst`.</span></span>|

## <a name="response"></a><span data-ttu-id="457ca-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="457ca-155">Response</span></span>

<span data-ttu-id="457ca-156">Se a exportação for iniciada com êxito, essa ação retornará um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="457ca-156">If the export is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="457ca-157">A resposta também conterá um header, que contém o local `Location` [do caseExportOperation](../resources/ediscovery-caseexportoperation.md) que foi criado para manipular a exportação.</span><span class="sxs-lookup"><span data-stu-id="457ca-157">The response will also contain a `Location` header, which contains the location of the [caseExportOperation](../resources/ediscovery-caseexportoperation.md) that was created to handle the export.</span></span> <span data-ttu-id="457ca-158">Verifique o status da operação de exportação fazendo uma solicitação GET para o local, quando concluído com êxito, o [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) mudará para `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="457ca-158">Check the status of the export operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="457ca-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="457ca-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="457ca-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="457ca-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reviewset_export"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/reviewsets/e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc/export
Content-Type: application/json
Content-length: 186

{
  "outputName": "2020-12-06 Contoso investigation export",
  "description": "Export for the Contoso investigation",
  "exportOptions": "originalFiles,fileInfo,tags",
  "exportStructure": "directory"
}
```

### <a name="response"></a><span data-ttu-id="457ca-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="457ca-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 3ec98906-7187-927e-5203-2ed4533175c6,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/operations('2ad2da7c7dbb404abfbbb28b7b6babd6'),
request-id: 9e6b9230-113c-49de-8f7d-ecb90d35b0de
```
