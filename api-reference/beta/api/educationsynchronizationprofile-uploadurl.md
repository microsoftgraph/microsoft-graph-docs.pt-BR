---
title: 'educationSynchronizationProfile: uploadUrl'
description: Recupere uma assinatura de acesso compartilhado (SAS) para carregar arquivos de origem para o armazenamento de blob do Azure para um perfil de sincronização de dados escolar específico no locatário. O token SAS tem uma validade de uma hora.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f37f5653147691c408cf83e3039920957352c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464695"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="484f8-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="484f8-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="484f8-105">Recupere uma assinatura de acesso compartilhado (SAS) para carregar arquivos de origem para o armazenamento de blob do Azure para um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="484f8-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="484f8-106">O token SAS tem uma validade de uma hora.</span><span class="sxs-lookup"><span data-stu-id="484f8-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="484f8-107">A URL de upload é fornecida somente para o [provedor de dados CSV](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="484f8-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="484f8-108">**Observação:** Para acessar o armazenamento de blob com o token SAS, use os [SDKs de armazenamento do Azure](https://github.com/search?q=org%3AAzure+azure-storage) ou o [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span><span class="sxs-lookup"><span data-stu-id="484f8-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="484f8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="484f8-109">Permissions</span></span>
<span data-ttu-id="484f8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="484f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="484f8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="484f8-112">Permission type</span></span> | <span data-ttu-id="484f8-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="484f8-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="484f8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="484f8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="484f8-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="484f8-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="484f8-116">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="484f8-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="484f8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="484f8-117">Not supported.</span></span>|
|<span data-ttu-id="484f8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="484f8-118">Application</span></span>|<span data-ttu-id="484f8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="484f8-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="484f8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="484f8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="484f8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="484f8-121">Request headers</span></span>
| <span data-ttu-id="484f8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="484f8-122">Name</span></span>       | <span data-ttu-id="484f8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="484f8-123">Type</span></span> | <span data-ttu-id="484f8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="484f8-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="484f8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="484f8-125">Authorization</span></span>  | <span data-ttu-id="484f8-126">string</span><span class="sxs-lookup"><span data-stu-id="484f8-126">string</span></span>  | <span data-ttu-id="484f8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="484f8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="484f8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="484f8-129">Request body</span></span>
<span data-ttu-id="484f8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="484f8-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="484f8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="484f8-131">Response</span></span>
<span data-ttu-id="484f8-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma URL SAS para o [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="484f8-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="484f8-133">Se uma solicitação anterior ainda estiver sendo processada, este método retornará `409 Conflict` um indicando que o carregamento está bloqueado atualmente para o [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="484f8-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="484f8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="484f8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="484f8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="484f8-135">Request</span></span>
<span data-ttu-id="484f8-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="484f8-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="484f8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="484f8-137">Response</span></span>
<span data-ttu-id="484f8-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="484f8-138">The following is an example of the response.</span></span> 

><span data-ttu-id="484f8-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="484f8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
