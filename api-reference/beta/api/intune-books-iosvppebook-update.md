---
title: Atualizar iosVppEBook
description: Atualiza as propriedades de um objeto iosVppEBook.
ms.openlocfilehash: c0b0b067eea640fe47367e7cbe1ff897e0ac8ef3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033322"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="2170b-103">Atualizar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="2170b-103">Update iosVppEBook</span></span>

> <span data-ttu-id="2170b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2170b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2170b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2170b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2170b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2170b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2170b-107">Atualizar as propriedades de um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="2170b-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2170b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2170b-108">Prerequisites</span></span>
<span data-ttu-id="2170b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2170b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2170b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2170b-111">Permission type</span></span>|<span data-ttu-id="2170b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2170b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2170b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2170b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2170b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2170b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2170b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2170b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2170b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2170b-116">Not supported.</span></span>|
|<span data-ttu-id="2170b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2170b-117">Application</span></span>|<span data-ttu-id="2170b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2170b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2170b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2170b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="2170b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2170b-120">Request headers</span></span>
|<span data-ttu-id="2170b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2170b-121">Header</span></span>|<span data-ttu-id="2170b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2170b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2170b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2170b-123">Authorization</span></span>|<span data-ttu-id="2170b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2170b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2170b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2170b-125">Accept</span></span>|<span data-ttu-id="2170b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2170b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2170b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2170b-127">Request body</span></span>
<span data-ttu-id="2170b-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="2170b-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="2170b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="2170b-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="2170b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2170b-130">Property</span></span>|<span data-ttu-id="2170b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2170b-131">Type</span></span>|<span data-ttu-id="2170b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2170b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2170b-133">id</span><span class="sxs-lookup"><span data-stu-id="2170b-133">id</span></span>|<span data-ttu-id="2170b-134">String</span><span class="sxs-lookup"><span data-stu-id="2170b-134">String</span></span>|<span data-ttu-id="2170b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2170b-135">Key of the entity.</span></span> <span data-ttu-id="2170b-136">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2170b-137">displayName</span></span>|<span data-ttu-id="2170b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2170b-138">String</span></span>|<span data-ttu-id="2170b-139">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2170b-139">Name of the eBook.</span></span> <span data-ttu-id="2170b-140">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-141">description</span><span class="sxs-lookup"><span data-stu-id="2170b-141">description</span></span>|<span data-ttu-id="2170b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2170b-142">String</span></span>|<span data-ttu-id="2170b-143">Descrição.</span><span class="sxs-lookup"><span data-stu-id="2170b-143">Description.</span></span> <span data-ttu-id="2170b-144">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2170b-145">publisher</span></span>|<span data-ttu-id="2170b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2170b-146">String</span></span>|<span data-ttu-id="2170b-147">Publicador.</span><span class="sxs-lookup"><span data-stu-id="2170b-147">Publisher.</span></span> <span data-ttu-id="2170b-148">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="2170b-149">publishedDateTime</span></span>|<span data-ttu-id="2170b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2170b-150">DateTimeOffset</span></span>|<span data-ttu-id="2170b-151">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="2170b-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="2170b-152">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="2170b-153">largeCover</span></span>|[<span data-ttu-id="2170b-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2170b-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2170b-155">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="2170b-155">Book cover.</span></span> <span data-ttu-id="2170b-156">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2170b-157">createdDateTime</span></span>|<span data-ttu-id="2170b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2170b-158">DateTimeOffset</span></span>|<span data-ttu-id="2170b-159">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2170b-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="2170b-160">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2170b-161">lastModifiedDateTime</span></span>|<span data-ttu-id="2170b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2170b-162">DateTimeOffset</span></span>|<span data-ttu-id="2170b-163">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="2170b-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="2170b-164">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2170b-165">informationUrl</span></span>|<span data-ttu-id="2170b-166">String</span><span class="sxs-lookup"><span data-stu-id="2170b-166">String</span></span>|<span data-ttu-id="2170b-167">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2170b-167">The more information Url.</span></span> <span data-ttu-id="2170b-168">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2170b-169">privacyInformationUrl</span></span>|<span data-ttu-id="2170b-170">String</span><span class="sxs-lookup"><span data-stu-id="2170b-170">String</span></span>|<span data-ttu-id="2170b-171">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2170b-171">The privacy statement Url.</span></span> <span data-ttu-id="2170b-172">Herdado de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2170b-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2170b-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2170b-173">vppTokenId</span></span>|<span data-ttu-id="2170b-174">Guid</span><span class="sxs-lookup"><span data-stu-id="2170b-174">Guid</span></span>|<span data-ttu-id="2170b-175">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="2170b-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="2170b-176">appleId</span><span class="sxs-lookup"><span data-stu-id="2170b-176">appleId</span></span>|<span data-ttu-id="2170b-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2170b-177">String</span></span>|<span data-ttu-id="2170b-178">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="2170b-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="2170b-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2170b-179">vppOrganizationName</span></span>|<span data-ttu-id="2170b-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2170b-180">String</span></span>|<span data-ttu-id="2170b-181">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="2170b-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="2170b-182">genres</span><span class="sxs-lookup"><span data-stu-id="2170b-182">genres</span></span>|<span data-ttu-id="2170b-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2170b-183">String collection</span></span>|<span data-ttu-id="2170b-184">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="2170b-184">Genres.</span></span>|
|<span data-ttu-id="2170b-185">idioma</span><span class="sxs-lookup"><span data-stu-id="2170b-185">language</span></span>|<span data-ttu-id="2170b-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2170b-186">String</span></span>|<span data-ttu-id="2170b-187">Idioma.</span><span class="sxs-lookup"><span data-stu-id="2170b-187">Language.</span></span>|
|<span data-ttu-id="2170b-188">seller</span><span class="sxs-lookup"><span data-stu-id="2170b-188">seller</span></span>|<span data-ttu-id="2170b-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2170b-189">String</span></span>|<span data-ttu-id="2170b-190">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="2170b-190">Seller.</span></span>|
|<span data-ttu-id="2170b-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2170b-191">totalLicenseCount</span></span>|<span data-ttu-id="2170b-192">Int32</span><span class="sxs-lookup"><span data-stu-id="2170b-192">Int32</span></span>|<span data-ttu-id="2170b-193">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="2170b-193">Total license count.</span></span>|
|<span data-ttu-id="2170b-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2170b-194">usedLicenseCount</span></span>|<span data-ttu-id="2170b-195">Int32</span><span class="sxs-lookup"><span data-stu-id="2170b-195">Int32</span></span>|<span data-ttu-id="2170b-196">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="2170b-196">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="2170b-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="2170b-197">Response</span></span>
<span data-ttu-id="2170b-198">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2170b-198">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2170b-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2170b-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="2170b-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2170b-200">Request</span></span>
<span data-ttu-id="2170b-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2170b-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 806

{
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

### <a name="response"></a><span data-ttu-id="2170b-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="2170b-202">Response</span></span>
<span data-ttu-id="2170b-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2170b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





