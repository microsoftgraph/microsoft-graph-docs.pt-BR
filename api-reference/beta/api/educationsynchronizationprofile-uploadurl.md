---
title: 'educationSynchronizationProfile: uploadUrl'
description: Recupere uma assinatura de acesso compartilhado (SAS) para o carregamento de arquivos de origem para o armazenamento de blob Azure para um perfil de sincronização de dados específicos escola no inquilino. O token SAS tem uma validade de uma hora.
author: mmast-msft
ms.openlocfilehash: 15a4536e21307067ac55783edd9eac675ae4144b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341059"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="cd6b7-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="cd6b7-104">educationSynchronizationProfile: uploadUrl</span></span>

> <span data-ttu-id="cd6b7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd6b7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd6b7-107">Recupere uma assinatura de acesso compartilhado (SAS) para carregar arquivos de origem para o armazenamento de blob Azure para um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-107">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="cd6b7-108">O token SAS tem uma validade de uma hora.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-108">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="cd6b7-109">O carregamento URL é fornecido apenas para o [provedor de dados CSV](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="cd6b7-109">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="cd6b7-110">**Observação:** Para acessar o armazenamento de blob com o token SAS, use o [armazenamento do Azure SDKs](https://github.com/search?q=org%3AAzure+azure-storage) ou [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span><span class="sxs-lookup"><span data-stu-id="cd6b7-110">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd6b7-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd6b7-111">Permissions</span></span>
<span data-ttu-id="cd6b7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd6b7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd6b7-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd6b7-114">Permission type</span></span> | <span data-ttu-id="cd6b7-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd6b7-115">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="cd6b7-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd6b7-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cd6b7-117">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd6b7-117">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="cd6b7-118">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="cd6b7-118">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cd6b7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-119">Not supported.</span></span>|
|<span data-ttu-id="cd6b7-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd6b7-120">Application</span></span>|<span data-ttu-id="cd6b7-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd6b7-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd6b7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="cd6b7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd6b7-123">Request headers</span></span>
| <span data-ttu-id="cd6b7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="cd6b7-124">Name</span></span>       | <span data-ttu-id="cd6b7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd6b7-125">Type</span></span> | <span data-ttu-id="cd6b7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd6b7-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd6b7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd6b7-127">Authorization</span></span>  | <span data-ttu-id="cd6b7-128">string</span><span class="sxs-lookup"><span data-stu-id="cd6b7-128">string</span></span>  | <span data-ttu-id="cd6b7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd6b7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd6b7-131">Request body</span></span>
<span data-ttu-id="cd6b7-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cd6b7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd6b7-133">Response</span></span>
<span data-ttu-id="cd6b7-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma URL de SAS para o [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-134">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="cd6b7-135">Se uma solicitação anterior ainda está sendo processada, esse método retorna um `409 Conflict` indicando que o carregamento momento seja bloqueado para o [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="cd6b7-135">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="cd6b7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd6b7-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd6b7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd6b7-137">Request</span></span>
<span data-ttu-id="cd6b7-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="cd6b7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd6b7-139">Response</span></span>
<span data-ttu-id="cd6b7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-140">The following is an example of the response.</span></span> 

><span data-ttu-id="cd6b7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd6b7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
