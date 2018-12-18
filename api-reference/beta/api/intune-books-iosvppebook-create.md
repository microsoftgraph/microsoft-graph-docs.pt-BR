---
title: Criar iosVppEBook
description: Cria um novo objeto iosVppEBook.
author: tfitzmac
ms.openlocfilehash: d50e698668c177069934fe6eb33aec4f3475fe17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314116"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="3c938-103">Criar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="3c938-103">Create iosVppEBook</span></span>

> <span data-ttu-id="3c938-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c938-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c938-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c938-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c938-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c938-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c938-107">Cria um novo objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="3c938-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c938-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c938-108">Prerequisites</span></span>
<span data-ttu-id="3c938-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c938-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c938-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c938-111">Permission type</span></span>|<span data-ttu-id="3c938-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c938-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c938-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c938-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c938-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c938-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c938-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c938-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c938-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c938-116">Not supported.</span></span>|
|<span data-ttu-id="3c938-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c938-117">Application</span></span>|<span data-ttu-id="3c938-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c938-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c938-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c938-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="3c938-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c938-120">Request headers</span></span>
|<span data-ttu-id="3c938-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c938-121">Header</span></span>|<span data-ttu-id="3c938-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3c938-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c938-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c938-123">Authorization</span></span>|<span data-ttu-id="3c938-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c938-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c938-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c938-125">Accept</span></span>|<span data-ttu-id="3c938-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c938-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c938-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c938-127">Request body</span></span>
<span data-ttu-id="3c938-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="3c938-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="3c938-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="3c938-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="3c938-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c938-130">Property</span></span>|<span data-ttu-id="3c938-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c938-131">Type</span></span>|<span data-ttu-id="3c938-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c938-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c938-133">id</span><span class="sxs-lookup"><span data-stu-id="3c938-133">id</span></span>|<span data-ttu-id="3c938-134">String</span><span class="sxs-lookup"><span data-stu-id="3c938-134">String</span></span>|<span data-ttu-id="3c938-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c938-135">Key of the entity.</span></span> <span data-ttu-id="3c938-136">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3c938-137">displayName</span></span>|<span data-ttu-id="3c938-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c938-138">String</span></span>|<span data-ttu-id="3c938-139">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="3c938-139">Name of the eBook.</span></span> <span data-ttu-id="3c938-140">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-141">description</span><span class="sxs-lookup"><span data-stu-id="3c938-141">description</span></span>|<span data-ttu-id="3c938-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c938-142">String</span></span>|<span data-ttu-id="3c938-143">Descrição.</span><span class="sxs-lookup"><span data-stu-id="3c938-143">Description.</span></span> <span data-ttu-id="3c938-144">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3c938-145">publisher</span></span>|<span data-ttu-id="3c938-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c938-146">String</span></span>|<span data-ttu-id="3c938-147">Publicador.</span><span class="sxs-lookup"><span data-stu-id="3c938-147">Publisher.</span></span> <span data-ttu-id="3c938-148">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c938-149">publishedDateTime</span></span>|<span data-ttu-id="3c938-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c938-150">DateTimeOffset</span></span>|<span data-ttu-id="3c938-151">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="3c938-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="3c938-152">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="3c938-153">largeCover</span></span>|[<span data-ttu-id="3c938-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3c938-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3c938-155">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="3c938-155">Book cover.</span></span> <span data-ttu-id="3c938-156">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c938-157">createdDateTime</span></span>|<span data-ttu-id="3c938-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c938-158">DateTimeOffset</span></span>|<span data-ttu-id="3c938-159">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3c938-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="3c938-160">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c938-161">lastModifiedDateTime</span></span>|<span data-ttu-id="3c938-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c938-162">DateTimeOffset</span></span>|<span data-ttu-id="3c938-163">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="3c938-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="3c938-164">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3c938-165">informationUrl</span></span>|<span data-ttu-id="3c938-166">String</span><span class="sxs-lookup"><span data-stu-id="3c938-166">String</span></span>|<span data-ttu-id="3c938-167">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3c938-167">The more information Url.</span></span> <span data-ttu-id="3c938-168">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3c938-169">privacyInformationUrl</span></span>|<span data-ttu-id="3c938-170">String</span><span class="sxs-lookup"><span data-stu-id="3c938-170">String</span></span>|<span data-ttu-id="3c938-171">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3c938-171">The privacy statement Url.</span></span> <span data-ttu-id="3c938-172">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3c938-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3c938-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="3c938-173">vppTokenId</span></span>|<span data-ttu-id="3c938-174">Guid</span><span class="sxs-lookup"><span data-stu-id="3c938-174">Guid</span></span>|<span data-ttu-id="3c938-175">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="3c938-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="3c938-176">appleId</span><span class="sxs-lookup"><span data-stu-id="3c938-176">appleId</span></span>|<span data-ttu-id="3c938-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c938-177">String</span></span>|<span data-ttu-id="3c938-178">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="3c938-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="3c938-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="3c938-179">vppOrganizationName</span></span>|<span data-ttu-id="3c938-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c938-180">String</span></span>|<span data-ttu-id="3c938-181">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="3c938-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="3c938-182">genres</span><span class="sxs-lookup"><span data-stu-id="3c938-182">genres</span></span>|<span data-ttu-id="3c938-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c938-183">String collection</span></span>|<span data-ttu-id="3c938-184">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="3c938-184">Genres.</span></span>|
|<span data-ttu-id="3c938-185">idioma</span><span class="sxs-lookup"><span data-stu-id="3c938-185">language</span></span>|<span data-ttu-id="3c938-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c938-186">String</span></span>|<span data-ttu-id="3c938-187">Idioma.</span><span class="sxs-lookup"><span data-stu-id="3c938-187">Language.</span></span>|
|<span data-ttu-id="3c938-188">seller</span><span class="sxs-lookup"><span data-stu-id="3c938-188">seller</span></span>|<span data-ttu-id="3c938-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c938-189">String</span></span>|<span data-ttu-id="3c938-190">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="3c938-190">Seller.</span></span>|
|<span data-ttu-id="3c938-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3c938-191">totalLicenseCount</span></span>|<span data-ttu-id="3c938-192">Int32</span><span class="sxs-lookup"><span data-stu-id="3c938-192">Int32</span></span>|<span data-ttu-id="3c938-193">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="3c938-193">Total license count.</span></span>|
|<span data-ttu-id="3c938-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3c938-194">usedLicenseCount</span></span>|<span data-ttu-id="3c938-195">Int32</span><span class="sxs-lookup"><span data-stu-id="3c938-195">Int32</span></span>|<span data-ttu-id="3c938-196">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="3c938-196">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="3c938-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c938-197">Response</span></span>
<span data-ttu-id="3c938-198">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c938-198">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c938-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c938-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c938-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c938-200">Request</span></span>
<span data-ttu-id="3c938-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c938-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 856

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

### <a name="response"></a><span data-ttu-id="3c938-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c938-202">Response</span></span>
<span data-ttu-id="3c938-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c938-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





