---
title: Criar microsoftStoreForBusinessApp
description: Cria um novo objeto microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7dccd660fb741254d4b600e73f35a17864a9ba29
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759767"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="dbf54-103">Criar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="dbf54-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="dbf54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbf54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbf54-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbf54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbf54-106">Cria um novo objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="dbf54-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbf54-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbf54-107">Prerequisites</span></span>
<span data-ttu-id="dbf54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbf54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbf54-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbf54-110">Permission type</span></span>|<span data-ttu-id="dbf54-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbf54-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbf54-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbf54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dbf54-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbf54-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dbf54-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbf54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbf54-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbf54-115">Not supported.</span></span>|
|<span data-ttu-id="dbf54-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbf54-116">Application</span></span>|<span data-ttu-id="dbf54-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbf54-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbf54-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbf54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="dbf54-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbf54-119">Request headers</span></span>
|<span data-ttu-id="dbf54-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbf54-120">Header</span></span>|<span data-ttu-id="dbf54-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dbf54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbf54-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbf54-122">Authorization</span></span>|<span data-ttu-id="dbf54-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbf54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbf54-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbf54-124">Accept</span></span>|<span data-ttu-id="dbf54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dbf54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbf54-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbf54-126">Request body</span></span>
<span data-ttu-id="dbf54-127">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="dbf54-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="dbf54-128">A tabela a seguir mostra as propriedades obrigatórias ao criar microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="dbf54-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="dbf54-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbf54-129">Property</span></span>|<span data-ttu-id="dbf54-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbf54-130">Type</span></span>|<span data-ttu-id="dbf54-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbf54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbf54-132">id</span><span class="sxs-lookup"><span data-stu-id="dbf54-132">id</span></span>|<span data-ttu-id="dbf54-133">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-133">String</span></span>|<span data-ttu-id="dbf54-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbf54-134">Key of the entity.</span></span> <span data-ttu-id="dbf54-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dbf54-136">displayName</span></span>|<span data-ttu-id="dbf54-137">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-137">String</span></span>|<span data-ttu-id="dbf54-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="dbf54-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dbf54-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-140">description</span><span class="sxs-lookup"><span data-stu-id="dbf54-140">description</span></span>|<span data-ttu-id="dbf54-141">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-141">String</span></span>|<span data-ttu-id="dbf54-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbf54-142">The description of the app.</span></span> <span data-ttu-id="dbf54-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-144">publicador</span><span class="sxs-lookup"><span data-stu-id="dbf54-144">publisher</span></span>|<span data-ttu-id="dbf54-145">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-145">String</span></span>|<span data-ttu-id="dbf54-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbf54-146">The publisher of the app.</span></span> <span data-ttu-id="dbf54-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dbf54-148">largeIcon</span></span>|[<span data-ttu-id="dbf54-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dbf54-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dbf54-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="dbf54-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dbf54-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dbf54-152">createdDateTime</span></span>|<span data-ttu-id="dbf54-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbf54-153">DateTimeOffset</span></span>|<span data-ttu-id="dbf54-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbf54-154">The date and time the app was created.</span></span> <span data-ttu-id="dbf54-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbf54-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dbf54-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbf54-157">DateTimeOffset</span></span>|<span data-ttu-id="dbf54-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="dbf54-158">The date and time the app was last modified.</span></span> <span data-ttu-id="dbf54-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dbf54-160">isFeatured</span></span>|<span data-ttu-id="dbf54-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbf54-161">Boolean</span></span>|<span data-ttu-id="dbf54-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dbf54-163">privacyInformationUrl</span></span>|<span data-ttu-id="dbf54-164">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-164">String</span></span>|<span data-ttu-id="dbf54-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="dbf54-165">The privacy statement Url.</span></span> <span data-ttu-id="dbf54-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dbf54-167">informationUrl</span></span>|<span data-ttu-id="dbf54-168">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-168">String</span></span>|<span data-ttu-id="dbf54-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="dbf54-169">The more information Url.</span></span> <span data-ttu-id="dbf54-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="dbf54-171">owner</span></span>|<span data-ttu-id="dbf54-172">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-172">String</span></span>|<span data-ttu-id="dbf54-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="dbf54-173">The owner of the app.</span></span> <span data-ttu-id="dbf54-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-175">developer</span><span class="sxs-lookup"><span data-stu-id="dbf54-175">developer</span></span>|<span data-ttu-id="dbf54-176">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-176">String</span></span>|<span data-ttu-id="dbf54-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbf54-177">The developer of the app.</span></span> <span data-ttu-id="dbf54-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-179">notes</span><span class="sxs-lookup"><span data-stu-id="dbf54-179">notes</span></span>|<span data-ttu-id="dbf54-180">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-180">String</span></span>|<span data-ttu-id="dbf54-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbf54-181">Notes for the app.</span></span> <span data-ttu-id="dbf54-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dbf54-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dbf54-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="dbf54-183">publishingState</span></span>|[<span data-ttu-id="dbf54-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dbf54-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dbf54-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbf54-185">The publishing state for the app.</span></span> <span data-ttu-id="dbf54-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="dbf54-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dbf54-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dbf54-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dbf54-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="dbf54-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dbf54-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dbf54-189">usedLicenseCount</span></span>|<span data-ttu-id="dbf54-190">Int32</span><span class="sxs-lookup"><span data-stu-id="dbf54-190">Int32</span></span>|<span data-ttu-id="dbf54-191">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="dbf54-191">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="dbf54-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dbf54-192">totalLicenseCount</span></span>|<span data-ttu-id="dbf54-193">Int32</span><span class="sxs-lookup"><span data-stu-id="dbf54-193">Int32</span></span>|<span data-ttu-id="dbf54-194">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="dbf54-194">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="dbf54-195">productKey</span><span class="sxs-lookup"><span data-stu-id="dbf54-195">productKey</span></span>|<span data-ttu-id="dbf54-196">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-196">String</span></span>|<span data-ttu-id="dbf54-197">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbf54-197">The app product key</span></span>|
|<span data-ttu-id="dbf54-198">licenseType</span><span class="sxs-lookup"><span data-stu-id="dbf54-198">licenseType</span></span>|[<span data-ttu-id="dbf54-199">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="dbf54-199">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="dbf54-200">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbf54-200">The app license type.</span></span> <span data-ttu-id="dbf54-201">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="dbf54-201">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="dbf54-202">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="dbf54-202">packageIdentityName</span></span>|<span data-ttu-id="dbf54-203">String</span><span class="sxs-lookup"><span data-stu-id="dbf54-203">String</span></span>|<span data-ttu-id="dbf54-204">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbf54-204">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="dbf54-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbf54-205">Response</span></span>
<span data-ttu-id="dbf54-206">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbf54-206">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbf54-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbf54-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbf54-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbf54-208">Request</span></span>
<span data-ttu-id="dbf54-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbf54-209">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dbf54-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbf54-210">Response</span></span>
<span data-ttu-id="dbf54-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbf54-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




