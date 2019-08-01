---
title: Atualizar iosVppEBook
description: Atualizar as propriedades de um objeto iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d68b8ba149b4b5f8b63029df98769d37a5fdd8c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001877"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="43d19-103">Atualizar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="43d19-103">Update iosVppEBook</span></span>

> <span data-ttu-id="43d19-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43d19-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43d19-105">Atualizar as propriedades de um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="43d19-105">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43d19-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43d19-106">Prerequisites</span></span>
<span data-ttu-id="43d19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43d19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43d19-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43d19-109">Permission type</span></span>|<span data-ttu-id="43d19-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43d19-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43d19-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43d19-111">Delegated (work or school account)</span></span>|<span data-ttu-id="43d19-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43d19-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43d19-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43d19-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43d19-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43d19-114">Not supported.</span></span>|
|<span data-ttu-id="43d19-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43d19-115">Application</span></span>|<span data-ttu-id="43d19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43d19-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43d19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43d19-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="43d19-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43d19-118">Request headers</span></span>
|<span data-ttu-id="43d19-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43d19-119">Header</span></span>|<span data-ttu-id="43d19-120">Valor</span><span class="sxs-lookup"><span data-stu-id="43d19-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43d19-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="43d19-121">Authorization</span></span>|<span data-ttu-id="43d19-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43d19-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43d19-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43d19-123">Accept</span></span>|<span data-ttu-id="43d19-124">application/json</span><span class="sxs-lookup"><span data-stu-id="43d19-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43d19-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43d19-125">Request body</span></span>
<span data-ttu-id="43d19-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="43d19-126">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="43d19-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="43d19-127">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="43d19-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43d19-128">Property</span></span>|<span data-ttu-id="43d19-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="43d19-129">Type</span></span>|<span data-ttu-id="43d19-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="43d19-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43d19-131">id</span><span class="sxs-lookup"><span data-stu-id="43d19-131">id</span></span>|<span data-ttu-id="43d19-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43d19-132">String</span></span>|<span data-ttu-id="43d19-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="43d19-133">Key of the entity.</span></span> <span data-ttu-id="43d19-134">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-135">displayName</span><span class="sxs-lookup"><span data-stu-id="43d19-135">displayName</span></span>|<span data-ttu-id="43d19-136">String</span><span class="sxs-lookup"><span data-stu-id="43d19-136">String</span></span>|<span data-ttu-id="43d19-137">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="43d19-137">Name of the eBook.</span></span> <span data-ttu-id="43d19-138">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-139">descrição</span><span class="sxs-lookup"><span data-stu-id="43d19-139">description</span></span>|<span data-ttu-id="43d19-140">String</span><span class="sxs-lookup"><span data-stu-id="43d19-140">String</span></span>|<span data-ttu-id="43d19-141">Descrição.</span><span class="sxs-lookup"><span data-stu-id="43d19-141">Description.</span></span> <span data-ttu-id="43d19-142">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-143">publisher</span><span class="sxs-lookup"><span data-stu-id="43d19-143">publisher</span></span>|<span data-ttu-id="43d19-144">String</span><span class="sxs-lookup"><span data-stu-id="43d19-144">String</span></span>|<span data-ttu-id="43d19-145">Publicador.</span><span class="sxs-lookup"><span data-stu-id="43d19-145">Publisher.</span></span> <span data-ttu-id="43d19-146">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="43d19-147">publishedDateTime</span></span>|<span data-ttu-id="43d19-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43d19-148">DateTimeOffset</span></span>|<span data-ttu-id="43d19-149">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="43d19-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="43d19-150">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="43d19-151">largeCover</span></span>|[<span data-ttu-id="43d19-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="43d19-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="43d19-153">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="43d19-153">Book cover.</span></span> <span data-ttu-id="43d19-154">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43d19-155">createdDateTime</span></span>|<span data-ttu-id="43d19-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43d19-156">DateTimeOffset</span></span>|<span data-ttu-id="43d19-157">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="43d19-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="43d19-158">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43d19-159">lastModifiedDateTime</span></span>|<span data-ttu-id="43d19-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43d19-160">DateTimeOffset</span></span>|<span data-ttu-id="43d19-161">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="43d19-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="43d19-162">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="43d19-163">informationUrl</span></span>|<span data-ttu-id="43d19-164">String</span><span class="sxs-lookup"><span data-stu-id="43d19-164">String</span></span>|<span data-ttu-id="43d19-165">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="43d19-165">The more information Url.</span></span> <span data-ttu-id="43d19-166">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="43d19-167">privacyInformationUrl</span></span>|<span data-ttu-id="43d19-168">String</span><span class="sxs-lookup"><span data-stu-id="43d19-168">String</span></span>|<span data-ttu-id="43d19-169">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="43d19-169">The privacy statement Url.</span></span> <span data-ttu-id="43d19-170">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="43d19-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="43d19-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="43d19-171">vppTokenId</span></span>|<span data-ttu-id="43d19-172">Guid</span><span class="sxs-lookup"><span data-stu-id="43d19-172">Guid</span></span>|<span data-ttu-id="43d19-173">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="43d19-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="43d19-174">appleId</span><span class="sxs-lookup"><span data-stu-id="43d19-174">appleId</span></span>|<span data-ttu-id="43d19-175">String</span><span class="sxs-lookup"><span data-stu-id="43d19-175">String</span></span>|<span data-ttu-id="43d19-176">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="43d19-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="43d19-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="43d19-177">vppOrganizationName</span></span>|<span data-ttu-id="43d19-178">String</span><span class="sxs-lookup"><span data-stu-id="43d19-178">String</span></span>|<span data-ttu-id="43d19-179">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="43d19-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="43d19-180">genres</span><span class="sxs-lookup"><span data-stu-id="43d19-180">genres</span></span>|<span data-ttu-id="43d19-181">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43d19-181">String collection</span></span>|<span data-ttu-id="43d19-182">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="43d19-182">Genres.</span></span>|
|<span data-ttu-id="43d19-183">idioma</span><span class="sxs-lookup"><span data-stu-id="43d19-183">language</span></span>|<span data-ttu-id="43d19-184">String</span><span class="sxs-lookup"><span data-stu-id="43d19-184">String</span></span>|<span data-ttu-id="43d19-185">Idioma.</span><span class="sxs-lookup"><span data-stu-id="43d19-185">Language.</span></span>|
|<span data-ttu-id="43d19-186">seller</span><span class="sxs-lookup"><span data-stu-id="43d19-186">seller</span></span>|<span data-ttu-id="43d19-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43d19-187">String</span></span>|<span data-ttu-id="43d19-188">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="43d19-188">Seller.</span></span>|
|<span data-ttu-id="43d19-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="43d19-189">totalLicenseCount</span></span>|<span data-ttu-id="43d19-190">Int32</span><span class="sxs-lookup"><span data-stu-id="43d19-190">Int32</span></span>|<span data-ttu-id="43d19-191">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="43d19-191">Total license count.</span></span>|
|<span data-ttu-id="43d19-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="43d19-192">usedLicenseCount</span></span>|<span data-ttu-id="43d19-193">Int32</span><span class="sxs-lookup"><span data-stu-id="43d19-193">Int32</span></span>|<span data-ttu-id="43d19-194">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="43d19-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="43d19-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="43d19-195">Response</span></span>
<span data-ttu-id="43d19-196">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43d19-196">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43d19-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43d19-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="43d19-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43d19-198">Request</span></span>
<span data-ttu-id="43d19-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43d19-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
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

### <a name="response"></a><span data-ttu-id="43d19-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="43d19-200">Response</span></span>
<span data-ttu-id="43d19-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43d19-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



