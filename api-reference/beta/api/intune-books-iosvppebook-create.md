---
title: Criar iosVppEBook
description: Cria um novo objeto iosVppEBook.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb641714a4ffbdb304ba3a95bb7078d9bc223696
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450360"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="62723-103">Criar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="62723-103">Create iosVppEBook</span></span>

<span data-ttu-id="62723-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="62723-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62723-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62723-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62723-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62723-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62723-107">Cria um novo objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="62723-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62723-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62723-108">Prerequisites</span></span>
<span data-ttu-id="62723-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62723-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62723-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62723-111">Permission type</span></span>|<span data-ttu-id="62723-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62723-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62723-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62723-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62723-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62723-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62723-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62723-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62723-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62723-116">Not supported.</span></span>|
|<span data-ttu-id="62723-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62723-117">Application</span></span>|<span data-ttu-id="62723-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62723-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62723-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62723-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="62723-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62723-120">Request headers</span></span>
|<span data-ttu-id="62723-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62723-121">Header</span></span>|<span data-ttu-id="62723-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62723-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62723-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62723-123">Authorization</span></span>|<span data-ttu-id="62723-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62723-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62723-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62723-125">Accept</span></span>|<span data-ttu-id="62723-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62723-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62723-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62723-127">Request body</span></span>
<span data-ttu-id="62723-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="62723-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="62723-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="62723-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="62723-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62723-130">Property</span></span>|<span data-ttu-id="62723-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="62723-131">Type</span></span>|<span data-ttu-id="62723-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="62723-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62723-133">id</span><span class="sxs-lookup"><span data-stu-id="62723-133">id</span></span>|<span data-ttu-id="62723-134">String</span><span class="sxs-lookup"><span data-stu-id="62723-134">String</span></span>|<span data-ttu-id="62723-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62723-135">Key of the entity.</span></span> <span data-ttu-id="62723-136">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-137">displayName</span><span class="sxs-lookup"><span data-stu-id="62723-137">displayName</span></span>|<span data-ttu-id="62723-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62723-138">String</span></span>|<span data-ttu-id="62723-139">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="62723-139">Name of the eBook.</span></span> <span data-ttu-id="62723-140">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-141">description</span><span class="sxs-lookup"><span data-stu-id="62723-141">description</span></span>|<span data-ttu-id="62723-142">String</span><span class="sxs-lookup"><span data-stu-id="62723-142">String</span></span>|<span data-ttu-id="62723-143">Descrição.</span><span class="sxs-lookup"><span data-stu-id="62723-143">Description.</span></span> <span data-ttu-id="62723-144">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-145">publisher</span><span class="sxs-lookup"><span data-stu-id="62723-145">publisher</span></span>|<span data-ttu-id="62723-146">String</span><span class="sxs-lookup"><span data-stu-id="62723-146">String</span></span>|<span data-ttu-id="62723-147">Publicador.</span><span class="sxs-lookup"><span data-stu-id="62723-147">Publisher.</span></span> <span data-ttu-id="62723-148">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="62723-149">publishedDateTime</span></span>|<span data-ttu-id="62723-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62723-150">DateTimeOffset</span></span>|<span data-ttu-id="62723-151">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="62723-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="62723-152">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="62723-153">largeCover</span></span>|[<span data-ttu-id="62723-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="62723-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="62723-155">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="62723-155">Book cover.</span></span> <span data-ttu-id="62723-156">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62723-157">createdDateTime</span></span>|<span data-ttu-id="62723-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62723-158">DateTimeOffset</span></span>|<span data-ttu-id="62723-159">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="62723-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="62723-160">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62723-161">lastModifiedDateTime</span></span>|<span data-ttu-id="62723-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62723-162">DateTimeOffset</span></span>|<span data-ttu-id="62723-163">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="62723-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="62723-164">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="62723-165">informationUrl</span></span>|<span data-ttu-id="62723-166">String</span><span class="sxs-lookup"><span data-stu-id="62723-166">String</span></span>|<span data-ttu-id="62723-167">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="62723-167">The more information Url.</span></span> <span data-ttu-id="62723-168">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="62723-169">privacyInformationUrl</span></span>|<span data-ttu-id="62723-170">String</span><span class="sxs-lookup"><span data-stu-id="62723-170">String</span></span>|<span data-ttu-id="62723-171">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="62723-171">The privacy statement Url.</span></span> <span data-ttu-id="62723-172">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="62723-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="62723-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="62723-173">vppTokenId</span></span>|<span data-ttu-id="62723-174">Guid</span><span class="sxs-lookup"><span data-stu-id="62723-174">Guid</span></span>|<span data-ttu-id="62723-175">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="62723-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="62723-176">appleId</span><span class="sxs-lookup"><span data-stu-id="62723-176">appleId</span></span>|<span data-ttu-id="62723-177">String</span><span class="sxs-lookup"><span data-stu-id="62723-177">String</span></span>|<span data-ttu-id="62723-178">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="62723-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="62723-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="62723-179">vppOrganizationName</span></span>|<span data-ttu-id="62723-180">String</span><span class="sxs-lookup"><span data-stu-id="62723-180">String</span></span>|<span data-ttu-id="62723-181">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="62723-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="62723-182">genres</span><span class="sxs-lookup"><span data-stu-id="62723-182">genres</span></span>|<span data-ttu-id="62723-183">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62723-183">String collection</span></span>|<span data-ttu-id="62723-184">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="62723-184">Genres.</span></span>|
|<span data-ttu-id="62723-185">idioma</span><span class="sxs-lookup"><span data-stu-id="62723-185">language</span></span>|<span data-ttu-id="62723-186">String</span><span class="sxs-lookup"><span data-stu-id="62723-186">String</span></span>|<span data-ttu-id="62723-187">Idioma.</span><span class="sxs-lookup"><span data-stu-id="62723-187">Language.</span></span>|
|<span data-ttu-id="62723-188">seller</span><span class="sxs-lookup"><span data-stu-id="62723-188">seller</span></span>|<span data-ttu-id="62723-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62723-189">String</span></span>|<span data-ttu-id="62723-190">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="62723-190">Seller.</span></span>|
|<span data-ttu-id="62723-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="62723-191">totalLicenseCount</span></span>|<span data-ttu-id="62723-192">Int32</span><span class="sxs-lookup"><span data-stu-id="62723-192">Int32</span></span>|<span data-ttu-id="62723-193">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="62723-193">Total license count.</span></span>|
|<span data-ttu-id="62723-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="62723-194">usedLicenseCount</span></span>|<span data-ttu-id="62723-195">Int32</span><span class="sxs-lookup"><span data-stu-id="62723-195">Int32</span></span>|<span data-ttu-id="62723-196">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="62723-196">Used license count.</span></span>|
|<span data-ttu-id="62723-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62723-197">roleScopeTagIds</span></span>|<span data-ttu-id="62723-198">String collection</span><span class="sxs-lookup"><span data-stu-id="62723-198">String collection</span></span>|<span data-ttu-id="62723-199">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="62723-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="62723-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="62723-200">Response</span></span>
<span data-ttu-id="62723-201">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62723-201">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62723-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62723-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="62723-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62723-203">Request</span></span>
<span data-ttu-id="62723-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62723-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62723-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="62723-205">Response</span></span>
<span data-ttu-id="62723-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62723-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





