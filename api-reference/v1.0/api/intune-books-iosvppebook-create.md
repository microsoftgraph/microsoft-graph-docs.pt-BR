---
title: Criar iosVppEBook
description: Cria um novo objeto iosVppEBook.
ms.openlocfilehash: e9a6802a25b76f62a6fc3960648b2265c3ea0de4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005417"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="370aa-103">Criar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="370aa-103">Create iosVppEBook</span></span>

> <span data-ttu-id="370aa-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="370aa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="370aa-105">Cria um novo objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="370aa-105">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="370aa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="370aa-106">Prerequisites</span></span>
<span data-ttu-id="370aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="370aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="370aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="370aa-109">Permission type</span></span>|<span data-ttu-id="370aa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="370aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="370aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="370aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="370aa-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="370aa-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="370aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="370aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="370aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="370aa-114">Not supported.</span></span>|
|<span data-ttu-id="370aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="370aa-115">Application</span></span>|<span data-ttu-id="370aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="370aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="370aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="370aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="370aa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="370aa-118">Request headers</span></span>
|<span data-ttu-id="370aa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="370aa-119">Header</span></span>|<span data-ttu-id="370aa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="370aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="370aa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="370aa-121">Authorization</span></span>|<span data-ttu-id="370aa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="370aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="370aa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="370aa-123">Accept</span></span>|<span data-ttu-id="370aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="370aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="370aa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="370aa-125">Request body</span></span>
<span data-ttu-id="370aa-126">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="370aa-126">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="370aa-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="370aa-127">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="370aa-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="370aa-128">Property</span></span>|<span data-ttu-id="370aa-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="370aa-129">Type</span></span>|<span data-ttu-id="370aa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="370aa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="370aa-131">id</span><span class="sxs-lookup"><span data-stu-id="370aa-131">id</span></span>|<span data-ttu-id="370aa-132">String</span><span class="sxs-lookup"><span data-stu-id="370aa-132">String</span></span>|<span data-ttu-id="370aa-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="370aa-133">Key of the entity.</span></span> <span data-ttu-id="370aa-134">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-135">displayName</span><span class="sxs-lookup"><span data-stu-id="370aa-135">displayName</span></span>|<span data-ttu-id="370aa-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="370aa-136">String</span></span>|<span data-ttu-id="370aa-137">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="370aa-137">Name of the eBook.</span></span> <span data-ttu-id="370aa-138">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-139">description</span><span class="sxs-lookup"><span data-stu-id="370aa-139">description</span></span>|<span data-ttu-id="370aa-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="370aa-140">String</span></span>|<span data-ttu-id="370aa-141">Descrição.</span><span class="sxs-lookup"><span data-stu-id="370aa-141">Description.</span></span> <span data-ttu-id="370aa-142">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-143">publisher</span><span class="sxs-lookup"><span data-stu-id="370aa-143">publisher</span></span>|<span data-ttu-id="370aa-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="370aa-144">String</span></span>|<span data-ttu-id="370aa-145">Publicador.</span><span class="sxs-lookup"><span data-stu-id="370aa-145">Publisher.</span></span> <span data-ttu-id="370aa-146">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="370aa-147">publishedDateTime</span></span>|<span data-ttu-id="370aa-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="370aa-148">DateTimeOffset</span></span>|<span data-ttu-id="370aa-149">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="370aa-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="370aa-150">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="370aa-151">largeCover</span></span>|[<span data-ttu-id="370aa-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="370aa-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="370aa-153">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="370aa-153">Book cover.</span></span> <span data-ttu-id="370aa-154">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="370aa-155">createdDateTime</span></span>|<span data-ttu-id="370aa-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="370aa-156">DateTimeOffset</span></span>|<span data-ttu-id="370aa-157">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="370aa-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="370aa-158">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="370aa-159">lastModifiedDateTime</span></span>|<span data-ttu-id="370aa-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="370aa-160">DateTimeOffset</span></span>|<span data-ttu-id="370aa-161">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="370aa-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="370aa-162">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="370aa-163">informationUrl</span></span>|<span data-ttu-id="370aa-164">String</span><span class="sxs-lookup"><span data-stu-id="370aa-164">String</span></span>|<span data-ttu-id="370aa-165">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="370aa-165">The more information Url.</span></span> <span data-ttu-id="370aa-166">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="370aa-167">privacyInformationUrl</span></span>|<span data-ttu-id="370aa-168">String</span><span class="sxs-lookup"><span data-stu-id="370aa-168">String</span></span>|<span data-ttu-id="370aa-169">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="370aa-169">The privacy statement Url.</span></span> <span data-ttu-id="370aa-170">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="370aa-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="370aa-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="370aa-171">vppTokenId</span></span>|<span data-ttu-id="370aa-172">Guid</span><span class="sxs-lookup"><span data-stu-id="370aa-172">Guid</span></span>|<span data-ttu-id="370aa-173">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="370aa-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="370aa-174">appleId</span><span class="sxs-lookup"><span data-stu-id="370aa-174">appleId</span></span>|<span data-ttu-id="370aa-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="370aa-175">String</span></span>|<span data-ttu-id="370aa-176">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="370aa-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="370aa-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="370aa-177">vppOrganizationName</span></span>|<span data-ttu-id="370aa-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="370aa-178">String</span></span>|<span data-ttu-id="370aa-179">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="370aa-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="370aa-180">genres</span><span class="sxs-lookup"><span data-stu-id="370aa-180">genres</span></span>|<span data-ttu-id="370aa-181">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="370aa-181">String collection</span></span>|<span data-ttu-id="370aa-182">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="370aa-182">Genres.</span></span>|
|<span data-ttu-id="370aa-183">idioma</span><span class="sxs-lookup"><span data-stu-id="370aa-183">language</span></span>|<span data-ttu-id="370aa-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="370aa-184">String</span></span>|<span data-ttu-id="370aa-185">Idioma.</span><span class="sxs-lookup"><span data-stu-id="370aa-185">Language.</span></span>|
|<span data-ttu-id="370aa-186">seller</span><span class="sxs-lookup"><span data-stu-id="370aa-186">seller</span></span>|<span data-ttu-id="370aa-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="370aa-187">String</span></span>|<span data-ttu-id="370aa-188">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="370aa-188">Seller.</span></span>|
|<span data-ttu-id="370aa-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="370aa-189">totalLicenseCount</span></span>|<span data-ttu-id="370aa-190">Int32</span><span class="sxs-lookup"><span data-stu-id="370aa-190">Int32</span></span>|<span data-ttu-id="370aa-191">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="370aa-191">Total license count.</span></span>|
|<span data-ttu-id="370aa-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="370aa-192">usedLicenseCount</span></span>|<span data-ttu-id="370aa-193">Int32</span><span class="sxs-lookup"><span data-stu-id="370aa-193">Int32</span></span>|<span data-ttu-id="370aa-194">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="370aa-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="370aa-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="370aa-195">Response</span></span>
<span data-ttu-id="370aa-196">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="370aa-196">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="370aa-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="370aa-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="370aa-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="370aa-198">Request</span></span>
<span data-ttu-id="370aa-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="370aa-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="370aa-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="370aa-200">Response</span></span>
<span data-ttu-id="370aa-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="370aa-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



