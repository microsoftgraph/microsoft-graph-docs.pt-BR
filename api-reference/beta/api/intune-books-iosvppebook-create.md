---
title: Criar iosVppEBook
description: Cria um novo objeto iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45edcdc7a31a6840da0b7af2ae5cf5e9618ad5d8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49245435"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="2336f-103">Criar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="2336f-103">Create iosVppEBook</span></span>

<span data-ttu-id="2336f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2336f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2336f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2336f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2336f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2336f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2336f-107">Cria um novo objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="2336f-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2336f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2336f-108">Prerequisites</span></span>
<span data-ttu-id="2336f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2336f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2336f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2336f-111">Permission type</span></span>|<span data-ttu-id="2336f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2336f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2336f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2336f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2336f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2336f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2336f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2336f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2336f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2336f-116">Not supported.</span></span>|
|<span data-ttu-id="2336f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2336f-117">Application</span></span>|<span data-ttu-id="2336f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2336f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2336f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2336f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="2336f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2336f-120">Request headers</span></span>
|<span data-ttu-id="2336f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2336f-121">Header</span></span>|<span data-ttu-id="2336f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2336f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2336f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2336f-123">Authorization</span></span>|<span data-ttu-id="2336f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2336f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2336f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2336f-125">Accept</span></span>|<span data-ttu-id="2336f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2336f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2336f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2336f-127">Request body</span></span>
<span data-ttu-id="2336f-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="2336f-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="2336f-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="2336f-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="2336f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2336f-130">Property</span></span>|<span data-ttu-id="2336f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2336f-131">Type</span></span>|<span data-ttu-id="2336f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2336f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2336f-133">id</span><span class="sxs-lookup"><span data-stu-id="2336f-133">id</span></span>|<span data-ttu-id="2336f-134">String</span><span class="sxs-lookup"><span data-stu-id="2336f-134">String</span></span>|<span data-ttu-id="2336f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2336f-135">Key of the entity.</span></span> <span data-ttu-id="2336f-136">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2336f-137">displayName</span></span>|<span data-ttu-id="2336f-138">String</span><span class="sxs-lookup"><span data-stu-id="2336f-138">String</span></span>|<span data-ttu-id="2336f-139">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2336f-139">Name of the eBook.</span></span> <span data-ttu-id="2336f-140">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-141">description</span><span class="sxs-lookup"><span data-stu-id="2336f-141">description</span></span>|<span data-ttu-id="2336f-142">String</span><span class="sxs-lookup"><span data-stu-id="2336f-142">String</span></span>|<span data-ttu-id="2336f-143">Descrição.</span><span class="sxs-lookup"><span data-stu-id="2336f-143">Description.</span></span> <span data-ttu-id="2336f-144">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2336f-145">publisher</span></span>|<span data-ttu-id="2336f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2336f-146">String</span></span>|<span data-ttu-id="2336f-147">Publicador.</span><span class="sxs-lookup"><span data-stu-id="2336f-147">Publisher.</span></span> <span data-ttu-id="2336f-148">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="2336f-149">publishedDateTime</span></span>|<span data-ttu-id="2336f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2336f-150">DateTimeOffset</span></span>|<span data-ttu-id="2336f-151">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="2336f-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="2336f-152">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="2336f-153">largeCover</span></span>|[<span data-ttu-id="2336f-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2336f-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2336f-155">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="2336f-155">Book cover.</span></span> <span data-ttu-id="2336f-156">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2336f-157">createdDateTime</span></span>|<span data-ttu-id="2336f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2336f-158">DateTimeOffset</span></span>|<span data-ttu-id="2336f-159">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2336f-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="2336f-160">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2336f-161">lastModifiedDateTime</span></span>|<span data-ttu-id="2336f-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2336f-162">DateTimeOffset</span></span>|<span data-ttu-id="2336f-163">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2336f-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="2336f-164">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2336f-165">informationUrl</span></span>|<span data-ttu-id="2336f-166">String</span><span class="sxs-lookup"><span data-stu-id="2336f-166">String</span></span>|<span data-ttu-id="2336f-167">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2336f-167">The more information Url.</span></span> <span data-ttu-id="2336f-168">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2336f-169">privacyInformationUrl</span></span>|<span data-ttu-id="2336f-170">String</span><span class="sxs-lookup"><span data-stu-id="2336f-170">String</span></span>|<span data-ttu-id="2336f-171">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2336f-171">The privacy statement Url.</span></span> <span data-ttu-id="2336f-172">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2336f-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2336f-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2336f-173">vppTokenId</span></span>|<span data-ttu-id="2336f-174">Guid</span><span class="sxs-lookup"><span data-stu-id="2336f-174">Guid</span></span>|<span data-ttu-id="2336f-175">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="2336f-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="2336f-176">appleId</span><span class="sxs-lookup"><span data-stu-id="2336f-176">appleId</span></span>|<span data-ttu-id="2336f-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2336f-177">String</span></span>|<span data-ttu-id="2336f-178">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="2336f-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="2336f-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2336f-179">vppOrganizationName</span></span>|<span data-ttu-id="2336f-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2336f-180">String</span></span>|<span data-ttu-id="2336f-181">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="2336f-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="2336f-182">genres</span><span class="sxs-lookup"><span data-stu-id="2336f-182">genres</span></span>|<span data-ttu-id="2336f-183">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2336f-183">String collection</span></span>|<span data-ttu-id="2336f-184">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="2336f-184">Genres.</span></span>|
|<span data-ttu-id="2336f-185">idioma</span><span class="sxs-lookup"><span data-stu-id="2336f-185">language</span></span>|<span data-ttu-id="2336f-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2336f-186">String</span></span>|<span data-ttu-id="2336f-187">Idioma.</span><span class="sxs-lookup"><span data-stu-id="2336f-187">Language.</span></span>|
|<span data-ttu-id="2336f-188">seller</span><span class="sxs-lookup"><span data-stu-id="2336f-188">seller</span></span>|<span data-ttu-id="2336f-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2336f-189">String</span></span>|<span data-ttu-id="2336f-190">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="2336f-190">Seller.</span></span>|
|<span data-ttu-id="2336f-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2336f-191">totalLicenseCount</span></span>|<span data-ttu-id="2336f-192">Int32</span><span class="sxs-lookup"><span data-stu-id="2336f-192">Int32</span></span>|<span data-ttu-id="2336f-193">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="2336f-193">Total license count.</span></span>|
|<span data-ttu-id="2336f-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2336f-194">usedLicenseCount</span></span>|<span data-ttu-id="2336f-195">Int32</span><span class="sxs-lookup"><span data-stu-id="2336f-195">Int32</span></span>|<span data-ttu-id="2336f-196">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="2336f-196">Used license count.</span></span>|
|<span data-ttu-id="2336f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2336f-197">roleScopeTagIds</span></span>|<span data-ttu-id="2336f-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2336f-198">String collection</span></span>|<span data-ttu-id="2336f-199">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2336f-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2336f-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="2336f-200">Response</span></span>
<span data-ttu-id="2336f-201">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2336f-201">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2336f-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2336f-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="2336f-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2336f-203">Request</span></span>
<span data-ttu-id="2336f-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2336f-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2336f-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="2336f-205">Response</span></span>
<span data-ttu-id="2336f-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2336f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




