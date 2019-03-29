---
title: Criar iosVppEBook
description: Cria um novo objeto iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9c481c036310ec3373fb280f356bfbbdb91d795
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973149"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="165cd-103">Criar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="165cd-103">Create iosVppEBook</span></span>

> <span data-ttu-id="165cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="165cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="165cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="165cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="165cd-106">Cria um novo objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="165cd-106">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="165cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="165cd-107">Prerequisites</span></span>
<span data-ttu-id="165cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="165cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="165cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="165cd-110">Permission type</span></span>|<span data-ttu-id="165cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="165cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="165cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="165cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="165cd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="165cd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="165cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="165cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="165cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="165cd-115">Not supported.</span></span>|
|<span data-ttu-id="165cd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="165cd-116">Application</span></span>|<span data-ttu-id="165cd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="165cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="165cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="165cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="165cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="165cd-119">Request headers</span></span>
|<span data-ttu-id="165cd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="165cd-120">Header</span></span>|<span data-ttu-id="165cd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="165cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="165cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="165cd-122">Authorization</span></span>|<span data-ttu-id="165cd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="165cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="165cd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="165cd-124">Accept</span></span>|<span data-ttu-id="165cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="165cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="165cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="165cd-126">Request body</span></span>
<span data-ttu-id="165cd-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="165cd-127">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="165cd-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="165cd-128">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="165cd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="165cd-129">Property</span></span>|<span data-ttu-id="165cd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="165cd-130">Type</span></span>|<span data-ttu-id="165cd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="165cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="165cd-132">id</span><span class="sxs-lookup"><span data-stu-id="165cd-132">id</span></span>|<span data-ttu-id="165cd-133">String</span><span class="sxs-lookup"><span data-stu-id="165cd-133">String</span></span>|<span data-ttu-id="165cd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="165cd-134">Key of the entity.</span></span> <span data-ttu-id="165cd-135">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="165cd-136">displayName</span></span>|<span data-ttu-id="165cd-137">String</span><span class="sxs-lookup"><span data-stu-id="165cd-137">String</span></span>|<span data-ttu-id="165cd-138">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="165cd-138">Name of the eBook.</span></span> <span data-ttu-id="165cd-139">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-140">descrição</span><span class="sxs-lookup"><span data-stu-id="165cd-140">description</span></span>|<span data-ttu-id="165cd-141">String</span><span class="sxs-lookup"><span data-stu-id="165cd-141">String</span></span>|<span data-ttu-id="165cd-142">Descrição.</span><span class="sxs-lookup"><span data-stu-id="165cd-142">Description.</span></span> <span data-ttu-id="165cd-143">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="165cd-144">publisher</span></span>|<span data-ttu-id="165cd-145">String</span><span class="sxs-lookup"><span data-stu-id="165cd-145">String</span></span>|<span data-ttu-id="165cd-146">Publicador.</span><span class="sxs-lookup"><span data-stu-id="165cd-146">Publisher.</span></span> <span data-ttu-id="165cd-147">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="165cd-148">publishedDateTime</span></span>|<span data-ttu-id="165cd-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="165cd-149">DateTimeOffset</span></span>|<span data-ttu-id="165cd-150">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="165cd-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="165cd-151">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="165cd-152">largeCover</span></span>|[<span data-ttu-id="165cd-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="165cd-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="165cd-154">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="165cd-154">Book cover.</span></span> <span data-ttu-id="165cd-155">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="165cd-156">createdDateTime</span></span>|<span data-ttu-id="165cd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="165cd-157">DateTimeOffset</span></span>|<span data-ttu-id="165cd-158">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="165cd-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="165cd-159">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="165cd-160">lastModifiedDateTime</span></span>|<span data-ttu-id="165cd-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="165cd-161">DateTimeOffset</span></span>|<span data-ttu-id="165cd-162">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="165cd-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="165cd-163">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="165cd-164">informationUrl</span></span>|<span data-ttu-id="165cd-165">String</span><span class="sxs-lookup"><span data-stu-id="165cd-165">String</span></span>|<span data-ttu-id="165cd-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="165cd-166">The more information Url.</span></span> <span data-ttu-id="165cd-167">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="165cd-168">privacyInformationUrl</span></span>|<span data-ttu-id="165cd-169">String</span><span class="sxs-lookup"><span data-stu-id="165cd-169">String</span></span>|<span data-ttu-id="165cd-170">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="165cd-170">The privacy statement Url.</span></span> <span data-ttu-id="165cd-171">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="165cd-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="165cd-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="165cd-172">vppTokenId</span></span>|<span data-ttu-id="165cd-173">Guid</span><span class="sxs-lookup"><span data-stu-id="165cd-173">Guid</span></span>|<span data-ttu-id="165cd-174">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="165cd-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="165cd-175">appleId</span><span class="sxs-lookup"><span data-stu-id="165cd-175">appleId</span></span>|<span data-ttu-id="165cd-176">String</span><span class="sxs-lookup"><span data-stu-id="165cd-176">String</span></span>|<span data-ttu-id="165cd-177">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="165cd-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="165cd-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="165cd-178">vppOrganizationName</span></span>|<span data-ttu-id="165cd-179">String</span><span class="sxs-lookup"><span data-stu-id="165cd-179">String</span></span>|<span data-ttu-id="165cd-180">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="165cd-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="165cd-181">genres</span><span class="sxs-lookup"><span data-stu-id="165cd-181">genres</span></span>|<span data-ttu-id="165cd-182">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="165cd-182">String collection</span></span>|<span data-ttu-id="165cd-183">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="165cd-183">Genres.</span></span>|
|<span data-ttu-id="165cd-184">idioma</span><span class="sxs-lookup"><span data-stu-id="165cd-184">language</span></span>|<span data-ttu-id="165cd-185">String</span><span class="sxs-lookup"><span data-stu-id="165cd-185">String</span></span>|<span data-ttu-id="165cd-186">Idioma.</span><span class="sxs-lookup"><span data-stu-id="165cd-186">Language.</span></span>|
|<span data-ttu-id="165cd-187">seller</span><span class="sxs-lookup"><span data-stu-id="165cd-187">seller</span></span>|<span data-ttu-id="165cd-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="165cd-188">String</span></span>|<span data-ttu-id="165cd-189">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="165cd-189">Seller.</span></span>|
|<span data-ttu-id="165cd-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="165cd-190">totalLicenseCount</span></span>|<span data-ttu-id="165cd-191">Int32</span><span class="sxs-lookup"><span data-stu-id="165cd-191">Int32</span></span>|<span data-ttu-id="165cd-192">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="165cd-192">Total license count.</span></span>|
|<span data-ttu-id="165cd-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="165cd-193">usedLicenseCount</span></span>|<span data-ttu-id="165cd-194">Int32</span><span class="sxs-lookup"><span data-stu-id="165cd-194">Int32</span></span>|<span data-ttu-id="165cd-195">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="165cd-195">Used license count.</span></span>|
|<span data-ttu-id="165cd-196">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="165cd-196">roleScopeTagIds</span></span>|<span data-ttu-id="165cd-197">Coleção String</span><span class="sxs-lookup"><span data-stu-id="165cd-197">String collection</span></span>|<span data-ttu-id="165cd-198">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="165cd-198">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="165cd-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="165cd-199">Response</span></span>
<span data-ttu-id="165cd-200">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="165cd-200">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="165cd-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="165cd-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="165cd-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="165cd-202">Request</span></span>
<span data-ttu-id="165cd-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="165cd-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="165cd-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="165cd-204">Response</span></span>
<span data-ttu-id="165cd-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="165cd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




