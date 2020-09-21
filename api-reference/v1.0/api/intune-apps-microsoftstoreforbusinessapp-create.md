---
title: Criar microsoftStoreForBusinessApp
description: Cria um novo objeto microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc3b4f8b4a7e82aa888cb4b843e15499724d6bec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073226"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="15788-103">Criar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="15788-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="15788-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15788-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15788-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15788-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15788-106">Cria um novo objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="15788-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15788-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15788-107">Prerequisites</span></span>
<span data-ttu-id="15788-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15788-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15788-110">Permission type</span></span>|<span data-ttu-id="15788-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15788-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15788-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15788-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15788-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15788-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="15788-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15788-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15788-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15788-115">Not supported.</span></span>|
|<span data-ttu-id="15788-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15788-116">Application</span></span>|<span data-ttu-id="15788-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15788-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15788-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15788-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="15788-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15788-119">Request headers</span></span>
|<span data-ttu-id="15788-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15788-120">Header</span></span>|<span data-ttu-id="15788-121">Valor</span><span class="sxs-lookup"><span data-stu-id="15788-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15788-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="15788-122">Authorization</span></span>|<span data-ttu-id="15788-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15788-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15788-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15788-124">Accept</span></span>|<span data-ttu-id="15788-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15788-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15788-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15788-126">Request body</span></span>
<span data-ttu-id="15788-127">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="15788-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="15788-128">A tabela a seguir mostra as propriedades obrigatórias ao criar microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="15788-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="15788-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15788-129">Property</span></span>|<span data-ttu-id="15788-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="15788-130">Type</span></span>|<span data-ttu-id="15788-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="15788-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15788-132">id</span><span class="sxs-lookup"><span data-stu-id="15788-132">id</span></span>|<span data-ttu-id="15788-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15788-133">String</span></span>|<span data-ttu-id="15788-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="15788-134">Key of the entity.</span></span> <span data-ttu-id="15788-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-136">displayName</span><span class="sxs-lookup"><span data-stu-id="15788-136">displayName</span></span>|<span data-ttu-id="15788-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15788-137">String</span></span>|<span data-ttu-id="15788-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="15788-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="15788-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-140">description</span><span class="sxs-lookup"><span data-stu-id="15788-140">description</span></span>|<span data-ttu-id="15788-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15788-141">String</span></span>|<span data-ttu-id="15788-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15788-142">The description of the app.</span></span> <span data-ttu-id="15788-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-144">publicador</span><span class="sxs-lookup"><span data-stu-id="15788-144">publisher</span></span>|<span data-ttu-id="15788-145">String</span><span class="sxs-lookup"><span data-stu-id="15788-145">String</span></span>|<span data-ttu-id="15788-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15788-146">The publisher of the app.</span></span> <span data-ttu-id="15788-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="15788-148">largeIcon</span></span>|[<span data-ttu-id="15788-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="15788-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="15788-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="15788-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="15788-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15788-152">createdDateTime</span></span>|<span data-ttu-id="15788-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15788-153">DateTimeOffset</span></span>|<span data-ttu-id="15788-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15788-154">The date and time the app was created.</span></span> <span data-ttu-id="15788-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15788-156">lastModifiedDateTime</span></span>|<span data-ttu-id="15788-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15788-157">DateTimeOffset</span></span>|<span data-ttu-id="15788-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="15788-158">The date and time the app was last modified.</span></span> <span data-ttu-id="15788-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="15788-160">isFeatured</span></span>|<span data-ttu-id="15788-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="15788-161">Boolean</span></span>|<span data-ttu-id="15788-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="15788-163">privacyInformationUrl</span></span>|<span data-ttu-id="15788-164">String</span><span class="sxs-lookup"><span data-stu-id="15788-164">String</span></span>|<span data-ttu-id="15788-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="15788-165">The privacy statement Url.</span></span> <span data-ttu-id="15788-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="15788-167">informationUrl</span></span>|<span data-ttu-id="15788-168">String</span><span class="sxs-lookup"><span data-stu-id="15788-168">String</span></span>|<span data-ttu-id="15788-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="15788-169">The more information Url.</span></span> <span data-ttu-id="15788-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-171">owner</span><span class="sxs-lookup"><span data-stu-id="15788-171">owner</span></span>|<span data-ttu-id="15788-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15788-172">String</span></span>|<span data-ttu-id="15788-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="15788-173">The owner of the app.</span></span> <span data-ttu-id="15788-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-175">developer</span><span class="sxs-lookup"><span data-stu-id="15788-175">developer</span></span>|<span data-ttu-id="15788-176">String</span><span class="sxs-lookup"><span data-stu-id="15788-176">String</span></span>|<span data-ttu-id="15788-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15788-177">The developer of the app.</span></span> <span data-ttu-id="15788-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-179">notes</span><span class="sxs-lookup"><span data-stu-id="15788-179">notes</span></span>|<span data-ttu-id="15788-180">String</span><span class="sxs-lookup"><span data-stu-id="15788-180">String</span></span>|<span data-ttu-id="15788-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15788-181">Notes for the app.</span></span> <span data-ttu-id="15788-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="15788-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="15788-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="15788-183">publishingState</span></span>|[<span data-ttu-id="15788-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="15788-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="15788-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15788-185">The publishing state for the app.</span></span> <span data-ttu-id="15788-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="15788-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="15788-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="15788-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="15788-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="15788-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="15788-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="15788-189">usedLicenseCount</span></span>|<span data-ttu-id="15788-190">Int32</span><span class="sxs-lookup"><span data-stu-id="15788-190">Int32</span></span>|<span data-ttu-id="15788-191">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="15788-191">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="15788-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="15788-192">totalLicenseCount</span></span>|<span data-ttu-id="15788-193">Int32</span><span class="sxs-lookup"><span data-stu-id="15788-193">Int32</span></span>|<span data-ttu-id="15788-194">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="15788-194">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="15788-195">productKey</span><span class="sxs-lookup"><span data-stu-id="15788-195">productKey</span></span>|<span data-ttu-id="15788-196">String</span><span class="sxs-lookup"><span data-stu-id="15788-196">String</span></span>|<span data-ttu-id="15788-197">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="15788-197">The app product key</span></span>|
|<span data-ttu-id="15788-198">licenseType</span><span class="sxs-lookup"><span data-stu-id="15788-198">licenseType</span></span>|[<span data-ttu-id="15788-199">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="15788-199">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="15788-200">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15788-200">The app license type.</span></span> <span data-ttu-id="15788-201">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="15788-201">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="15788-202">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="15788-202">packageIdentityName</span></span>|<span data-ttu-id="15788-203">String</span><span class="sxs-lookup"><span data-stu-id="15788-203">String</span></span>|<span data-ttu-id="15788-204">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="15788-204">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="15788-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="15788-205">Response</span></span>
<span data-ttu-id="15788-206">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15788-206">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15788-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15788-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="15788-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15788-208">Request</span></span>
<span data-ttu-id="15788-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15788-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="15788-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="15788-210">Response</span></span>
<span data-ttu-id="15788-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15788-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```









