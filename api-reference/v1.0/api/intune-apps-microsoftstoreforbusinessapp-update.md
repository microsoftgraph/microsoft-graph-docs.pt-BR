---
title: Atualizar microsoftStoreForBusinessApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5463470cc0fd9fb67fc693b2678cfa190fdefe91
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411644"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="3f459-103">Atualizar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="3f459-103">Update microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="3f459-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f459-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f459-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f459-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f459-106">Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="3f459-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f459-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3f459-107">Prerequisites</span></span>
<span data-ttu-id="3f459-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f459-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f459-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f459-110">Permission type</span></span>|<span data-ttu-id="3f459-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3f459-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f459-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f459-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f459-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f459-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3f459-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f459-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f459-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f459-115">Not supported.</span></span>|
|<span data-ttu-id="3f459-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f459-116">Application</span></span>|<span data-ttu-id="3f459-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f459-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f459-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f459-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="3f459-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f459-119">Request headers</span></span>
|<span data-ttu-id="3f459-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f459-120">Header</span></span>|<span data-ttu-id="3f459-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3f459-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f459-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f459-122">Authorization</span></span>|<span data-ttu-id="3f459-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f459-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f459-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3f459-124">Accept</span></span>|<span data-ttu-id="3f459-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f459-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f459-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f459-126">Request body</span></span>
<span data-ttu-id="3f459-127">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="3f459-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="3f459-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="3f459-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="3f459-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f459-129">Property</span></span>|<span data-ttu-id="3f459-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f459-130">Type</span></span>|<span data-ttu-id="3f459-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f459-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f459-132">id</span><span class="sxs-lookup"><span data-stu-id="3f459-132">id</span></span>|<span data-ttu-id="3f459-133">String</span><span class="sxs-lookup"><span data-stu-id="3f459-133">String</span></span>|<span data-ttu-id="3f459-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3f459-134">Key of the entity.</span></span> <span data-ttu-id="3f459-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3f459-136">displayName</span></span>|<span data-ttu-id="3f459-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f459-137">String</span></span>|<span data-ttu-id="3f459-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3f459-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3f459-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-140">description</span><span class="sxs-lookup"><span data-stu-id="3f459-140">description</span></span>|<span data-ttu-id="3f459-141">String</span><span class="sxs-lookup"><span data-stu-id="3f459-141">String</span></span>|<span data-ttu-id="3f459-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f459-142">The description of the app.</span></span> <span data-ttu-id="3f459-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-144">publicador</span><span class="sxs-lookup"><span data-stu-id="3f459-144">publisher</span></span>|<span data-ttu-id="3f459-145">String</span><span class="sxs-lookup"><span data-stu-id="3f459-145">String</span></span>|<span data-ttu-id="3f459-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f459-146">The publisher of the app.</span></span> <span data-ttu-id="3f459-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3f459-148">largeIcon</span></span>|[<span data-ttu-id="3f459-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3f459-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3f459-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3f459-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3f459-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f459-152">createdDateTime</span></span>|<span data-ttu-id="3f459-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f459-153">DateTimeOffset</span></span>|<span data-ttu-id="3f459-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f459-154">The date and time the app was created.</span></span> <span data-ttu-id="3f459-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f459-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3f459-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f459-157">DateTimeOffset</span></span>|<span data-ttu-id="3f459-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3f459-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3f459-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3f459-160">isFeatured</span></span>|<span data-ttu-id="3f459-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f459-161">Boolean</span></span>|<span data-ttu-id="3f459-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3f459-163">privacyInformationUrl</span></span>|<span data-ttu-id="3f459-164">String</span><span class="sxs-lookup"><span data-stu-id="3f459-164">String</span></span>|<span data-ttu-id="3f459-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3f459-165">The privacy statement Url.</span></span> <span data-ttu-id="3f459-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3f459-167">informationUrl</span></span>|<span data-ttu-id="3f459-168">String</span><span class="sxs-lookup"><span data-stu-id="3f459-168">String</span></span>|<span data-ttu-id="3f459-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3f459-169">The more information Url.</span></span> <span data-ttu-id="3f459-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-171">owner</span><span class="sxs-lookup"><span data-stu-id="3f459-171">owner</span></span>|<span data-ttu-id="3f459-172">String</span><span class="sxs-lookup"><span data-stu-id="3f459-172">String</span></span>|<span data-ttu-id="3f459-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3f459-173">The owner of the app.</span></span> <span data-ttu-id="3f459-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-175">developer</span><span class="sxs-lookup"><span data-stu-id="3f459-175">developer</span></span>|<span data-ttu-id="3f459-176">String</span><span class="sxs-lookup"><span data-stu-id="3f459-176">String</span></span>|<span data-ttu-id="3f459-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f459-177">The developer of the app.</span></span> <span data-ttu-id="3f459-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-179">notes</span><span class="sxs-lookup"><span data-stu-id="3f459-179">notes</span></span>|<span data-ttu-id="3f459-180">String</span><span class="sxs-lookup"><span data-stu-id="3f459-180">String</span></span>|<span data-ttu-id="3f459-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f459-181">Notes for the app.</span></span> <span data-ttu-id="3f459-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3f459-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3f459-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="3f459-183">publishingState</span></span>|[<span data-ttu-id="3f459-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3f459-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3f459-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f459-185">The publishing state for the app.</span></span> <span data-ttu-id="3f459-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3f459-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3f459-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3f459-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3f459-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3f459-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3f459-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3f459-189">usedLicenseCount</span></span>|<span data-ttu-id="3f459-190">Int32</span><span class="sxs-lookup"><span data-stu-id="3f459-190">Int32</span></span>|<span data-ttu-id="3f459-191">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="3f459-191">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="3f459-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3f459-192">totalLicenseCount</span></span>|<span data-ttu-id="3f459-193">Int32</span><span class="sxs-lookup"><span data-stu-id="3f459-193">Int32</span></span>|<span data-ttu-id="3f459-194">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="3f459-194">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="3f459-195">productKey</span><span class="sxs-lookup"><span data-stu-id="3f459-195">productKey</span></span>|<span data-ttu-id="3f459-196">String</span><span class="sxs-lookup"><span data-stu-id="3f459-196">String</span></span>|<span data-ttu-id="3f459-197">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f459-197">The app product key</span></span>|
|<span data-ttu-id="3f459-198">licenseType</span><span class="sxs-lookup"><span data-stu-id="3f459-198">licenseType</span></span>|[<span data-ttu-id="3f459-199">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="3f459-199">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="3f459-200">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f459-200">The app license type.</span></span> <span data-ttu-id="3f459-201">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="3f459-201">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="3f459-202">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="3f459-202">packageIdentityName</span></span>|<span data-ttu-id="3f459-203">String</span><span class="sxs-lookup"><span data-stu-id="3f459-203">String</span></span>|<span data-ttu-id="3f459-204">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f459-204">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="3f459-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f459-205">Response</span></span>
<span data-ttu-id="3f459-206">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f459-206">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f459-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f459-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f459-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f459-208">Request</span></span>
<span data-ttu-id="3f459-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f459-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="3f459-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f459-210">Response</span></span>
<span data-ttu-id="3f459-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f459-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






