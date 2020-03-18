---
title: Criar iosVppEBook
description: Cria um novo objeto iosVppEBook.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cd7c521ed2cfd8587262d0056eccc00a5bee76ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760505"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="67855-103">Criar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="67855-103">Create iosVppEBook</span></span>

> <span data-ttu-id="67855-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67855-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67855-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67855-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67855-106">Cria um novo objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="67855-106">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67855-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67855-107">Prerequisites</span></span>
<span data-ttu-id="67855-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67855-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67855-110">Permission type</span></span>|<span data-ttu-id="67855-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67855-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67855-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67855-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67855-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67855-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67855-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67855-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67855-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67855-115">Not supported.</span></span>|
|<span data-ttu-id="67855-116">Application</span><span class="sxs-lookup"><span data-stu-id="67855-116">Application</span></span>|<span data-ttu-id="67855-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67855-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67855-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67855-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="67855-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67855-119">Request headers</span></span>
|<span data-ttu-id="67855-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67855-120">Header</span></span>|<span data-ttu-id="67855-121">Valor</span><span class="sxs-lookup"><span data-stu-id="67855-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67855-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="67855-122">Authorization</span></span>|<span data-ttu-id="67855-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67855-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67855-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67855-124">Accept</span></span>|<span data-ttu-id="67855-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67855-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67855-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67855-126">Request body</span></span>
<span data-ttu-id="67855-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="67855-127">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="67855-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="67855-128">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="67855-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67855-129">Property</span></span>|<span data-ttu-id="67855-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="67855-130">Type</span></span>|<span data-ttu-id="67855-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="67855-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67855-132">id</span><span class="sxs-lookup"><span data-stu-id="67855-132">id</span></span>|<span data-ttu-id="67855-133">String</span><span class="sxs-lookup"><span data-stu-id="67855-133">String</span></span>|<span data-ttu-id="67855-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67855-134">Key of the entity.</span></span> <span data-ttu-id="67855-135">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-136">displayName</span><span class="sxs-lookup"><span data-stu-id="67855-136">displayName</span></span>|<span data-ttu-id="67855-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67855-137">String</span></span>|<span data-ttu-id="67855-138">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="67855-138">Name of the eBook.</span></span> <span data-ttu-id="67855-139">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-140">description</span><span class="sxs-lookup"><span data-stu-id="67855-140">description</span></span>|<span data-ttu-id="67855-141">String</span><span class="sxs-lookup"><span data-stu-id="67855-141">String</span></span>|<span data-ttu-id="67855-142">Descrição.</span><span class="sxs-lookup"><span data-stu-id="67855-142">Description.</span></span> <span data-ttu-id="67855-143">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-144">publisher</span><span class="sxs-lookup"><span data-stu-id="67855-144">publisher</span></span>|<span data-ttu-id="67855-145">String</span><span class="sxs-lookup"><span data-stu-id="67855-145">String</span></span>|<span data-ttu-id="67855-146">Publicador.</span><span class="sxs-lookup"><span data-stu-id="67855-146">Publisher.</span></span> <span data-ttu-id="67855-147">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="67855-148">publishedDateTime</span></span>|<span data-ttu-id="67855-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67855-149">DateTimeOffset</span></span>|<span data-ttu-id="67855-150">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="67855-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="67855-151">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="67855-152">largeCover</span></span>|[<span data-ttu-id="67855-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="67855-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="67855-154">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="67855-154">Book cover.</span></span> <span data-ttu-id="67855-155">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67855-156">createdDateTime</span></span>|<span data-ttu-id="67855-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67855-157">DateTimeOffset</span></span>|<span data-ttu-id="67855-158">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="67855-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="67855-159">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67855-160">lastModifiedDateTime</span></span>|<span data-ttu-id="67855-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67855-161">DateTimeOffset</span></span>|<span data-ttu-id="67855-162">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="67855-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="67855-163">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="67855-164">informationUrl</span></span>|<span data-ttu-id="67855-165">String</span><span class="sxs-lookup"><span data-stu-id="67855-165">String</span></span>|<span data-ttu-id="67855-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="67855-166">The more information Url.</span></span> <span data-ttu-id="67855-167">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="67855-168">privacyInformationUrl</span></span>|<span data-ttu-id="67855-169">String</span><span class="sxs-lookup"><span data-stu-id="67855-169">String</span></span>|<span data-ttu-id="67855-170">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="67855-170">The privacy statement Url.</span></span> <span data-ttu-id="67855-171">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="67855-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67855-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="67855-172">vppTokenId</span></span>|<span data-ttu-id="67855-173">Guid</span><span class="sxs-lookup"><span data-stu-id="67855-173">Guid</span></span>|<span data-ttu-id="67855-174">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="67855-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="67855-175">appleId</span><span class="sxs-lookup"><span data-stu-id="67855-175">appleId</span></span>|<span data-ttu-id="67855-176">String</span><span class="sxs-lookup"><span data-stu-id="67855-176">String</span></span>|<span data-ttu-id="67855-177">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="67855-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="67855-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="67855-178">vppOrganizationName</span></span>|<span data-ttu-id="67855-179">String</span><span class="sxs-lookup"><span data-stu-id="67855-179">String</span></span>|<span data-ttu-id="67855-180">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="67855-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="67855-181">genres</span><span class="sxs-lookup"><span data-stu-id="67855-181">genres</span></span>|<span data-ttu-id="67855-182">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67855-182">String collection</span></span>|<span data-ttu-id="67855-183">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="67855-183">Genres.</span></span>|
|<span data-ttu-id="67855-184">idioma</span><span class="sxs-lookup"><span data-stu-id="67855-184">language</span></span>|<span data-ttu-id="67855-185">String</span><span class="sxs-lookup"><span data-stu-id="67855-185">String</span></span>|<span data-ttu-id="67855-186">Idioma.</span><span class="sxs-lookup"><span data-stu-id="67855-186">Language.</span></span>|
|<span data-ttu-id="67855-187">seller</span><span class="sxs-lookup"><span data-stu-id="67855-187">seller</span></span>|<span data-ttu-id="67855-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67855-188">String</span></span>|<span data-ttu-id="67855-189">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="67855-189">Seller.</span></span>|
|<span data-ttu-id="67855-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67855-190">totalLicenseCount</span></span>|<span data-ttu-id="67855-191">Int32</span><span class="sxs-lookup"><span data-stu-id="67855-191">Int32</span></span>|<span data-ttu-id="67855-192">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="67855-192">Total license count.</span></span>|
|<span data-ttu-id="67855-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67855-193">usedLicenseCount</span></span>|<span data-ttu-id="67855-194">Int32</span><span class="sxs-lookup"><span data-stu-id="67855-194">Int32</span></span>|<span data-ttu-id="67855-195">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="67855-195">Used license count.</span></span>|
|<span data-ttu-id="67855-196">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67855-196">roleScopeTagIds</span></span>|<span data-ttu-id="67855-197">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="67855-197">String collection</span></span>|<span data-ttu-id="67855-198">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="67855-198">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="67855-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="67855-199">Response</span></span>
<span data-ttu-id="67855-200">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67855-200">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67855-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67855-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="67855-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67855-202">Request</span></span>
<span data-ttu-id="67855-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67855-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 854

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="67855-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="67855-204">Response</span></span>
<span data-ttu-id="67855-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67855-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1026

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




