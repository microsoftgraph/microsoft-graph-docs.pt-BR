---
title: Atualizar iosVppEBook
description: Atualizar as propriedades de um objeto iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 348874662bf7ce1e05c661df50c8f6b5ba5a227a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48716156"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="893e2-103">Atualizar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="893e2-103">Update iosVppEBook</span></span>

<span data-ttu-id="893e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="893e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="893e2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="893e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="893e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="893e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="893e2-107">Atualizar as propriedades de um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="893e2-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="893e2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="893e2-108">Prerequisites</span></span>
<span data-ttu-id="893e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="893e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="893e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="893e2-111">Permission type</span></span>|<span data-ttu-id="893e2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="893e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="893e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="893e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="893e2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="893e2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="893e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="893e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="893e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="893e2-116">Not supported.</span></span>|
|<span data-ttu-id="893e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="893e2-117">Application</span></span>|<span data-ttu-id="893e2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="893e2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="893e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="893e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="893e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="893e2-120">Request headers</span></span>
|<span data-ttu-id="893e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="893e2-121">Header</span></span>|<span data-ttu-id="893e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="893e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="893e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="893e2-123">Authorization</span></span>|<span data-ttu-id="893e2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="893e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="893e2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="893e2-125">Accept</span></span>|<span data-ttu-id="893e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="893e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="893e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="893e2-127">Request body</span></span>
<span data-ttu-id="893e2-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="893e2-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="893e2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="893e2-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="893e2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="893e2-130">Property</span></span>|<span data-ttu-id="893e2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="893e2-131">Type</span></span>|<span data-ttu-id="893e2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="893e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="893e2-133">id</span><span class="sxs-lookup"><span data-stu-id="893e2-133">id</span></span>|<span data-ttu-id="893e2-134">String</span><span class="sxs-lookup"><span data-stu-id="893e2-134">String</span></span>|<span data-ttu-id="893e2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="893e2-135">Key of the entity.</span></span> <span data-ttu-id="893e2-136">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="893e2-137">displayName</span></span>|<span data-ttu-id="893e2-138">String</span><span class="sxs-lookup"><span data-stu-id="893e2-138">String</span></span>|<span data-ttu-id="893e2-139">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="893e2-139">Name of the eBook.</span></span> <span data-ttu-id="893e2-140">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-141">description</span><span class="sxs-lookup"><span data-stu-id="893e2-141">description</span></span>|<span data-ttu-id="893e2-142">String</span><span class="sxs-lookup"><span data-stu-id="893e2-142">String</span></span>|<span data-ttu-id="893e2-143">Descrição.</span><span class="sxs-lookup"><span data-stu-id="893e2-143">Description.</span></span> <span data-ttu-id="893e2-144">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="893e2-145">publisher</span></span>|<span data-ttu-id="893e2-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="893e2-146">String</span></span>|<span data-ttu-id="893e2-147">Publicador.</span><span class="sxs-lookup"><span data-stu-id="893e2-147">Publisher.</span></span> <span data-ttu-id="893e2-148">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="893e2-149">publishedDateTime</span></span>|<span data-ttu-id="893e2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="893e2-150">DateTimeOffset</span></span>|<span data-ttu-id="893e2-151">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="893e2-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="893e2-152">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="893e2-153">largeCover</span></span>|[<span data-ttu-id="893e2-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="893e2-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="893e2-155">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="893e2-155">Book cover.</span></span> <span data-ttu-id="893e2-156">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="893e2-157">createdDateTime</span></span>|<span data-ttu-id="893e2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="893e2-158">DateTimeOffset</span></span>|<span data-ttu-id="893e2-159">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="893e2-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="893e2-160">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="893e2-161">lastModifiedDateTime</span></span>|<span data-ttu-id="893e2-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="893e2-162">DateTimeOffset</span></span>|<span data-ttu-id="893e2-163">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="893e2-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="893e2-164">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="893e2-165">informationUrl</span></span>|<span data-ttu-id="893e2-166">String</span><span class="sxs-lookup"><span data-stu-id="893e2-166">String</span></span>|<span data-ttu-id="893e2-167">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="893e2-167">The more information Url.</span></span> <span data-ttu-id="893e2-168">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="893e2-169">privacyInformationUrl</span></span>|<span data-ttu-id="893e2-170">String</span><span class="sxs-lookup"><span data-stu-id="893e2-170">String</span></span>|<span data-ttu-id="893e2-171">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="893e2-171">The privacy statement Url.</span></span> <span data-ttu-id="893e2-172">Herdada de [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="893e2-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="893e2-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="893e2-173">vppTokenId</span></span>|<span data-ttu-id="893e2-174">Guid</span><span class="sxs-lookup"><span data-stu-id="893e2-174">Guid</span></span>|<span data-ttu-id="893e2-175">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="893e2-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="893e2-176">appleId</span><span class="sxs-lookup"><span data-stu-id="893e2-176">appleId</span></span>|<span data-ttu-id="893e2-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="893e2-177">String</span></span>|<span data-ttu-id="893e2-178">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="893e2-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="893e2-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="893e2-179">vppOrganizationName</span></span>|<span data-ttu-id="893e2-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="893e2-180">String</span></span>|<span data-ttu-id="893e2-181">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="893e2-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="893e2-182">genres</span><span class="sxs-lookup"><span data-stu-id="893e2-182">genres</span></span>|<span data-ttu-id="893e2-183">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="893e2-183">String collection</span></span>|<span data-ttu-id="893e2-184">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="893e2-184">Genres.</span></span>|
|<span data-ttu-id="893e2-185">idioma</span><span class="sxs-lookup"><span data-stu-id="893e2-185">language</span></span>|<span data-ttu-id="893e2-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="893e2-186">String</span></span>|<span data-ttu-id="893e2-187">Idioma.</span><span class="sxs-lookup"><span data-stu-id="893e2-187">Language.</span></span>|
|<span data-ttu-id="893e2-188">seller</span><span class="sxs-lookup"><span data-stu-id="893e2-188">seller</span></span>|<span data-ttu-id="893e2-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="893e2-189">String</span></span>|<span data-ttu-id="893e2-190">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="893e2-190">Seller.</span></span>|
|<span data-ttu-id="893e2-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="893e2-191">totalLicenseCount</span></span>|<span data-ttu-id="893e2-192">Int32</span><span class="sxs-lookup"><span data-stu-id="893e2-192">Int32</span></span>|<span data-ttu-id="893e2-193">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="893e2-193">Total license count.</span></span>|
|<span data-ttu-id="893e2-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="893e2-194">usedLicenseCount</span></span>|<span data-ttu-id="893e2-195">Int32</span><span class="sxs-lookup"><span data-stu-id="893e2-195">Int32</span></span>|<span data-ttu-id="893e2-196">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="893e2-196">Used license count.</span></span>|
|<span data-ttu-id="893e2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="893e2-197">roleScopeTagIds</span></span>|<span data-ttu-id="893e2-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="893e2-198">String collection</span></span>|<span data-ttu-id="893e2-199">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="893e2-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="893e2-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="893e2-200">Response</span></span>
<span data-ttu-id="893e2-201">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="893e2-201">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="893e2-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="893e2-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="893e2-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="893e2-203">Request</span></span>
<span data-ttu-id="893e2-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="893e2-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="893e2-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="893e2-205">Response</span></span>
<span data-ttu-id="893e2-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="893e2-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





