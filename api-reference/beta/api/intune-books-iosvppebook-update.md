---
title: Atualizar iosVppEBook
description: Atualizar as propriedades de um objeto iosVppEBook.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75923333d699e4cd8cd24a223231d3b720aea542
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328449"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="93593-103">Atualizar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="93593-103">Update iosVppEBook</span></span>

> <span data-ttu-id="93593-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93593-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93593-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93593-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93593-106">Atualizar as propriedades de um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="93593-106">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93593-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93593-107">Prerequisites</span></span>
<span data-ttu-id="93593-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93593-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93593-110">Permission type</span></span>|<span data-ttu-id="93593-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93593-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93593-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93593-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93593-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93593-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="93593-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93593-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93593-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93593-115">Not supported.</span></span>|
|<span data-ttu-id="93593-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93593-116">Application</span></span>|<span data-ttu-id="93593-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93593-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93593-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93593-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="93593-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93593-119">Request headers</span></span>
|<span data-ttu-id="93593-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93593-120">Header</span></span>|<span data-ttu-id="93593-121">Valor</span><span class="sxs-lookup"><span data-stu-id="93593-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93593-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="93593-122">Authorization</span></span>|<span data-ttu-id="93593-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93593-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93593-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93593-124">Accept</span></span>|<span data-ttu-id="93593-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93593-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93593-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93593-126">Request body</span></span>
<span data-ttu-id="93593-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="93593-127">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="93593-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="93593-128">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="93593-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93593-129">Property</span></span>|<span data-ttu-id="93593-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="93593-130">Type</span></span>|<span data-ttu-id="93593-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="93593-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93593-132">id</span><span class="sxs-lookup"><span data-stu-id="93593-132">id</span></span>|<span data-ttu-id="93593-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93593-133">String</span></span>|<span data-ttu-id="93593-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="93593-134">Key of the entity.</span></span> <span data-ttu-id="93593-135">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-136">displayName</span><span class="sxs-lookup"><span data-stu-id="93593-136">displayName</span></span>|<span data-ttu-id="93593-137">String</span><span class="sxs-lookup"><span data-stu-id="93593-137">String</span></span>|<span data-ttu-id="93593-138">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="93593-138">Name of the eBook.</span></span> <span data-ttu-id="93593-139">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-140">descrição</span><span class="sxs-lookup"><span data-stu-id="93593-140">description</span></span>|<span data-ttu-id="93593-141">String</span><span class="sxs-lookup"><span data-stu-id="93593-141">String</span></span>|<span data-ttu-id="93593-142">Descrição.</span><span class="sxs-lookup"><span data-stu-id="93593-142">Description.</span></span> <span data-ttu-id="93593-143">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-144">publisher</span><span class="sxs-lookup"><span data-stu-id="93593-144">publisher</span></span>|<span data-ttu-id="93593-145">String</span><span class="sxs-lookup"><span data-stu-id="93593-145">String</span></span>|<span data-ttu-id="93593-146">Publicador.</span><span class="sxs-lookup"><span data-stu-id="93593-146">Publisher.</span></span> <span data-ttu-id="93593-147">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="93593-148">publishedDateTime</span></span>|<span data-ttu-id="93593-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93593-149">DateTimeOffset</span></span>|<span data-ttu-id="93593-150">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="93593-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="93593-151">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="93593-152">largeCover</span></span>|[<span data-ttu-id="93593-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="93593-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="93593-154">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="93593-154">Book cover.</span></span> <span data-ttu-id="93593-155">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93593-156">createdDateTime</span></span>|<span data-ttu-id="93593-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93593-157">DateTimeOffset</span></span>|<span data-ttu-id="93593-158">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="93593-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="93593-159">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93593-160">lastModifiedDateTime</span></span>|<span data-ttu-id="93593-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93593-161">DateTimeOffset</span></span>|<span data-ttu-id="93593-162">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="93593-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="93593-163">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="93593-164">informationUrl</span></span>|<span data-ttu-id="93593-165">String</span><span class="sxs-lookup"><span data-stu-id="93593-165">String</span></span>|<span data-ttu-id="93593-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="93593-166">The more information Url.</span></span> <span data-ttu-id="93593-167">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="93593-168">privacyInformationUrl</span></span>|<span data-ttu-id="93593-169">String</span><span class="sxs-lookup"><span data-stu-id="93593-169">String</span></span>|<span data-ttu-id="93593-170">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="93593-170">The privacy statement Url.</span></span> <span data-ttu-id="93593-171">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="93593-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="93593-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="93593-172">vppTokenId</span></span>|<span data-ttu-id="93593-173">Guid</span><span class="sxs-lookup"><span data-stu-id="93593-173">Guid</span></span>|<span data-ttu-id="93593-174">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="93593-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="93593-175">appleId</span><span class="sxs-lookup"><span data-stu-id="93593-175">appleId</span></span>|<span data-ttu-id="93593-176">String</span><span class="sxs-lookup"><span data-stu-id="93593-176">String</span></span>|<span data-ttu-id="93593-177">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="93593-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="93593-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="93593-178">vppOrganizationName</span></span>|<span data-ttu-id="93593-179">String</span><span class="sxs-lookup"><span data-stu-id="93593-179">String</span></span>|<span data-ttu-id="93593-180">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="93593-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="93593-181">genres</span><span class="sxs-lookup"><span data-stu-id="93593-181">genres</span></span>|<span data-ttu-id="93593-182">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93593-182">String collection</span></span>|<span data-ttu-id="93593-183">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="93593-183">Genres.</span></span>|
|<span data-ttu-id="93593-184">idioma</span><span class="sxs-lookup"><span data-stu-id="93593-184">language</span></span>|<span data-ttu-id="93593-185">String</span><span class="sxs-lookup"><span data-stu-id="93593-185">String</span></span>|<span data-ttu-id="93593-186">Idioma.</span><span class="sxs-lookup"><span data-stu-id="93593-186">Language.</span></span>|
|<span data-ttu-id="93593-187">seller</span><span class="sxs-lookup"><span data-stu-id="93593-187">seller</span></span>|<span data-ttu-id="93593-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93593-188">String</span></span>|<span data-ttu-id="93593-189">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="93593-189">Seller.</span></span>|
|<span data-ttu-id="93593-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="93593-190">totalLicenseCount</span></span>|<span data-ttu-id="93593-191">Int32</span><span class="sxs-lookup"><span data-stu-id="93593-191">Int32</span></span>|<span data-ttu-id="93593-192">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="93593-192">Total license count.</span></span>|
|<span data-ttu-id="93593-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="93593-193">usedLicenseCount</span></span>|<span data-ttu-id="93593-194">Int32</span><span class="sxs-lookup"><span data-stu-id="93593-194">Int32</span></span>|<span data-ttu-id="93593-195">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="93593-195">Used license count.</span></span>|
|<span data-ttu-id="93593-196">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93593-196">roleScopeTagIds</span></span>|<span data-ttu-id="93593-197">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93593-197">String collection</span></span>|<span data-ttu-id="93593-198">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="93593-198">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="93593-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="93593-199">Response</span></span>
<span data-ttu-id="93593-200">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93593-200">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93593-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93593-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="93593-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93593-202">Request</span></span>
<span data-ttu-id="93593-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93593-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
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

### <a name="response"></a><span data-ttu-id="93593-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="93593-204">Response</span></span>
<span data-ttu-id="93593-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93593-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






