---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 940c87cb1b3b5dc7ff7f1731b97bcfdbb4a0e2be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516381"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="18549-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="18549-103">Update managedAndroidStoreApp</span></span>

<span data-ttu-id="18549-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18549-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18549-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18549-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18549-106">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="18549-106">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18549-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18549-107">Prerequisites</span></span>
<span data-ttu-id="18549-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18549-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18549-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18549-110">Permission type</span></span>|<span data-ttu-id="18549-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18549-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18549-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18549-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18549-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18549-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18549-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18549-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18549-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18549-115">Not supported.</span></span>|
|<span data-ttu-id="18549-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18549-116">Application</span></span>|<span data-ttu-id="18549-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18549-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18549-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18549-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="18549-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18549-119">Request headers</span></span>
|<span data-ttu-id="18549-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18549-120">Header</span></span>|<span data-ttu-id="18549-121">Valor</span><span class="sxs-lookup"><span data-stu-id="18549-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18549-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18549-122">Authorization</span></span>|<span data-ttu-id="18549-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18549-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18549-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18549-124">Accept</span></span>|<span data-ttu-id="18549-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18549-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18549-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18549-126">Request body</span></span>
<span data-ttu-id="18549-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="18549-127">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="18549-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="18549-128">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="18549-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18549-129">Property</span></span>|<span data-ttu-id="18549-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="18549-130">Type</span></span>|<span data-ttu-id="18549-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="18549-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18549-132">id</span><span class="sxs-lookup"><span data-stu-id="18549-132">id</span></span>|<span data-ttu-id="18549-133">String</span><span class="sxs-lookup"><span data-stu-id="18549-133">String</span></span>|<span data-ttu-id="18549-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18549-134">Key of the entity.</span></span> <span data-ttu-id="18549-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-136">displayName</span><span class="sxs-lookup"><span data-stu-id="18549-136">displayName</span></span>|<span data-ttu-id="18549-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18549-137">String</span></span>|<span data-ttu-id="18549-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="18549-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="18549-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-140">description</span><span class="sxs-lookup"><span data-stu-id="18549-140">description</span></span>|<span data-ttu-id="18549-141">String</span><span class="sxs-lookup"><span data-stu-id="18549-141">String</span></span>|<span data-ttu-id="18549-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-142">The description of the app.</span></span> <span data-ttu-id="18549-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-144">publicador</span><span class="sxs-lookup"><span data-stu-id="18549-144">publisher</span></span>|<span data-ttu-id="18549-145">String</span><span class="sxs-lookup"><span data-stu-id="18549-145">String</span></span>|<span data-ttu-id="18549-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-146">The publisher of the app.</span></span> <span data-ttu-id="18549-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="18549-148">largeIcon</span></span>|[<span data-ttu-id="18549-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18549-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18549-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="18549-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="18549-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18549-152">createdDateTime</span></span>|<span data-ttu-id="18549-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18549-153">DateTimeOffset</span></span>|<span data-ttu-id="18549-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-154">The date and time the app was created.</span></span> <span data-ttu-id="18549-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18549-156">lastModifiedDateTime</span></span>|<span data-ttu-id="18549-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18549-157">DateTimeOffset</span></span>|<span data-ttu-id="18549-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="18549-158">The date and time the app was last modified.</span></span> <span data-ttu-id="18549-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="18549-160">isFeatured</span></span>|<span data-ttu-id="18549-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="18549-161">Boolean</span></span>|<span data-ttu-id="18549-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18549-163">privacyInformationUrl</span></span>|<span data-ttu-id="18549-164">String</span><span class="sxs-lookup"><span data-stu-id="18549-164">String</span></span>|<span data-ttu-id="18549-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="18549-165">The privacy statement Url.</span></span> <span data-ttu-id="18549-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18549-167">informationUrl</span></span>|<span data-ttu-id="18549-168">String</span><span class="sxs-lookup"><span data-stu-id="18549-168">String</span></span>|<span data-ttu-id="18549-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="18549-169">The more information Url.</span></span> <span data-ttu-id="18549-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-171">owner</span><span class="sxs-lookup"><span data-stu-id="18549-171">owner</span></span>|<span data-ttu-id="18549-172">String</span><span class="sxs-lookup"><span data-stu-id="18549-172">String</span></span>|<span data-ttu-id="18549-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="18549-173">The owner of the app.</span></span> <span data-ttu-id="18549-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-175">developer</span><span class="sxs-lookup"><span data-stu-id="18549-175">developer</span></span>|<span data-ttu-id="18549-176">String</span><span class="sxs-lookup"><span data-stu-id="18549-176">String</span></span>|<span data-ttu-id="18549-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-177">The developer of the app.</span></span> <span data-ttu-id="18549-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-179">notes</span><span class="sxs-lookup"><span data-stu-id="18549-179">notes</span></span>|<span data-ttu-id="18549-180">String</span><span class="sxs-lookup"><span data-stu-id="18549-180">String</span></span>|<span data-ttu-id="18549-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-181">Notes for the app.</span></span> <span data-ttu-id="18549-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18549-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="18549-183">publishingState</span></span>|[<span data-ttu-id="18549-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="18549-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="18549-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-185">The publishing state for the app.</span></span> <span data-ttu-id="18549-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="18549-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="18549-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18549-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="18549-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="18549-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="18549-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="18549-189">appAvailability</span></span>|[<span data-ttu-id="18549-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="18549-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="18549-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-191">The Application's availability.</span></span> <span data-ttu-id="18549-192">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="18549-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="18549-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="18549-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="18549-194">version</span><span class="sxs-lookup"><span data-stu-id="18549-194">version</span></span>|<span data-ttu-id="18549-195">String</span><span class="sxs-lookup"><span data-stu-id="18549-195">String</span></span>|<span data-ttu-id="18549-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-196">The Application's version.</span></span> <span data-ttu-id="18549-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="18549-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="18549-198">packageId</span><span class="sxs-lookup"><span data-stu-id="18549-198">packageId</span></span>|<span data-ttu-id="18549-199">String</span><span class="sxs-lookup"><span data-stu-id="18549-199">String</span></span>|<span data-ttu-id="18549-200">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18549-200">The app's package ID.</span></span>|
|<span data-ttu-id="18549-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="18549-201">appStoreUrl</span></span>|<span data-ttu-id="18549-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18549-202">String</span></span>|<span data-ttu-id="18549-203">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="18549-203">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="18549-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18549-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="18549-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18549-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="18549-206">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="18549-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="18549-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="18549-207">Response</span></span>
<span data-ttu-id="18549-208">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18549-208">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18549-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18549-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="18549-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18549-210">Request</span></span>
<span data-ttu-id="18549-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18549-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1016

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="18549-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="18549-212">Response</span></span>
<span data-ttu-id="18549-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18549-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1188

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```




