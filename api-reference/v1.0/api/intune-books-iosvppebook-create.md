---
title: Criar iosVppEBook
description: Cria um novo objeto iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6251e3ecda1597653ff2fed9575e7357e89f652f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577102"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="dbfdd-103">Criar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="dbfdd-103">Create iosVppEBook</span></span>

> <span data-ttu-id="dbfdd-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbfdd-105">Cria um novo objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="dbfdd-105">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbfdd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbfdd-106">Prerequisites</span></span>
<span data-ttu-id="dbfdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbfdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbfdd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbfdd-109">Permission type</span></span>|<span data-ttu-id="dbfdd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbfdd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dbfdd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbfdd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dbfdd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbfdd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-114">Not supported.</span></span>|
|<span data-ttu-id="dbfdd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbfdd-115">Application</span></span>|<span data-ttu-id="dbfdd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbfdd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbfdd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="dbfdd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbfdd-118">Request headers</span></span>
|<span data-ttu-id="dbfdd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbfdd-119">Header</span></span>|<span data-ttu-id="dbfdd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dbfdd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbfdd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbfdd-121">Authorization</span></span>|<span data-ttu-id="dbfdd-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbfdd-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbfdd-123">Accept</span></span>|<span data-ttu-id="dbfdd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dbfdd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbfdd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbfdd-125">Request body</span></span>
<span data-ttu-id="dbfdd-126">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-126">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="dbfdd-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-127">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="dbfdd-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbfdd-128">Property</span></span>|<span data-ttu-id="dbfdd-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbfdd-129">Type</span></span>|<span data-ttu-id="dbfdd-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbfdd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbfdd-131">id</span><span class="sxs-lookup"><span data-stu-id="dbfdd-131">id</span></span>|<span data-ttu-id="dbfdd-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbfdd-132">String</span></span>|<span data-ttu-id="dbfdd-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-133">Key of the entity.</span></span> <span data-ttu-id="dbfdd-134">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dbfdd-135">displayName</span></span>|<span data-ttu-id="dbfdd-136">String</span><span class="sxs-lookup"><span data-stu-id="dbfdd-136">String</span></span>|<span data-ttu-id="dbfdd-137">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-137">Name of the eBook.</span></span> <span data-ttu-id="dbfdd-138">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-139">description</span><span class="sxs-lookup"><span data-stu-id="dbfdd-139">description</span></span>|<span data-ttu-id="dbfdd-140">String</span><span class="sxs-lookup"><span data-stu-id="dbfdd-140">String</span></span>|<span data-ttu-id="dbfdd-141">Descrição.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-141">Description.</span></span> <span data-ttu-id="dbfdd-142">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-143">publisher</span><span class="sxs-lookup"><span data-stu-id="dbfdd-143">publisher</span></span>|<span data-ttu-id="dbfdd-144">String</span><span class="sxs-lookup"><span data-stu-id="dbfdd-144">String</span></span>|<span data-ttu-id="dbfdd-145">Publicador.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-145">Publisher.</span></span> <span data-ttu-id="dbfdd-146">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbfdd-147">publishedDateTime</span></span>|<span data-ttu-id="dbfdd-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbfdd-148">DateTimeOffset</span></span>|<span data-ttu-id="dbfdd-149">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="dbfdd-150">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="dbfdd-151">largeCover</span></span>|[<span data-ttu-id="dbfdd-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dbfdd-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dbfdd-153">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-153">Book cover.</span></span> <span data-ttu-id="dbfdd-154">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dbfdd-155">createdDateTime</span></span>|<span data-ttu-id="dbfdd-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbfdd-156">DateTimeOffset</span></span>|<span data-ttu-id="dbfdd-157">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="dbfdd-158">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbfdd-159">lastModifiedDateTime</span></span>|<span data-ttu-id="dbfdd-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbfdd-160">DateTimeOffset</span></span>|<span data-ttu-id="dbfdd-161">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="dbfdd-162">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dbfdd-163">informationUrl</span></span>|<span data-ttu-id="dbfdd-164">String</span><span class="sxs-lookup"><span data-stu-id="dbfdd-164">String</span></span>|<span data-ttu-id="dbfdd-165">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-165">The more information Url.</span></span> <span data-ttu-id="dbfdd-166">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dbfdd-167">privacyInformationUrl</span></span>|<span data-ttu-id="dbfdd-168">String</span><span class="sxs-lookup"><span data-stu-id="dbfdd-168">String</span></span>|<span data-ttu-id="dbfdd-169">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-169">The privacy statement Url.</span></span> <span data-ttu-id="dbfdd-170">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="dbfdd-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="dbfdd-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="dbfdd-171">vppTokenId</span></span>|<span data-ttu-id="dbfdd-172">Guid</span><span class="sxs-lookup"><span data-stu-id="dbfdd-172">Guid</span></span>|<span data-ttu-id="dbfdd-173">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="dbfdd-174">appleId</span><span class="sxs-lookup"><span data-stu-id="dbfdd-174">appleId</span></span>|<span data-ttu-id="dbfdd-175">String</span><span class="sxs-lookup"><span data-stu-id="dbfdd-175">String</span></span>|<span data-ttu-id="dbfdd-176">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="dbfdd-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="dbfdd-177">vppOrganizationName</span></span>|<span data-ttu-id="dbfdd-178">String</span><span class="sxs-lookup"><span data-stu-id="dbfdd-178">String</span></span>|<span data-ttu-id="dbfdd-179">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="dbfdd-180">genres</span><span class="sxs-lookup"><span data-stu-id="dbfdd-180">genres</span></span>|<span data-ttu-id="dbfdd-181">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbfdd-181">String collection</span></span>|<span data-ttu-id="dbfdd-182">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-182">Genres.</span></span>|
|<span data-ttu-id="dbfdd-183">idioma</span><span class="sxs-lookup"><span data-stu-id="dbfdd-183">language</span></span>|<span data-ttu-id="dbfdd-184">String</span><span class="sxs-lookup"><span data-stu-id="dbfdd-184">String</span></span>|<span data-ttu-id="dbfdd-185">Idioma.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-185">Language.</span></span>|
|<span data-ttu-id="dbfdd-186">seller</span><span class="sxs-lookup"><span data-stu-id="dbfdd-186">seller</span></span>|<span data-ttu-id="dbfdd-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbfdd-187">String</span></span>|<span data-ttu-id="dbfdd-188">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-188">Seller.</span></span>|
|<span data-ttu-id="dbfdd-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dbfdd-189">totalLicenseCount</span></span>|<span data-ttu-id="dbfdd-190">Int32</span><span class="sxs-lookup"><span data-stu-id="dbfdd-190">Int32</span></span>|<span data-ttu-id="dbfdd-191">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-191">Total license count.</span></span>|
|<span data-ttu-id="dbfdd-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dbfdd-192">usedLicenseCount</span></span>|<span data-ttu-id="dbfdd-193">Int32</span><span class="sxs-lookup"><span data-stu-id="dbfdd-193">Int32</span></span>|<span data-ttu-id="dbfdd-194">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="dbfdd-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbfdd-195">Response</span></span>
<span data-ttu-id="dbfdd-196">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-196">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbfdd-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbfdd-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbfdd-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbfdd-198">Request</span></span>
<span data-ttu-id="dbfdd-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 792

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
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="dbfdd-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbfdd-200">Response</span></span>
<span data-ttu-id="dbfdd-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbfdd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

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
  "usedLicenseCount": 0
}
```



