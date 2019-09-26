---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96dcc2cdd5c257d44ce62ea6e95abf1210960e1c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196116"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="cdace-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="cdace-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="cdace-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdace-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdace-105">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdace-105">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdace-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cdace-106">Prerequisites</span></span>
<span data-ttu-id="cdace-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cdace-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cdace-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdace-109">Permission type</span></span>|<span data-ttu-id="cdace-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cdace-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdace-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdace-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdace-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdace-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cdace-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdace-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdace-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdace-114">Not supported.</span></span>|
|<span data-ttu-id="cdace-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdace-115">Application</span></span>|<span data-ttu-id="cdace-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdace-116">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdace-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdace-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cdace-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdace-118">Request headers</span></span>
|<span data-ttu-id="cdace-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdace-119">Header</span></span>|<span data-ttu-id="cdace-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cdace-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdace-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdace-121">Authorization</span></span>|<span data-ttu-id="cdace-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdace-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdace-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cdace-123">Accept</span></span>|<span data-ttu-id="cdace-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cdace-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdace-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdace-125">Request body</span></span>
<span data-ttu-id="cdace-126">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="cdace-126">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="cdace-127">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="cdace-127">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="cdace-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdace-128">Property</span></span>|<span data-ttu-id="cdace-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdace-129">Type</span></span>|<span data-ttu-id="cdace-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdace-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdace-131">id</span><span class="sxs-lookup"><span data-stu-id="cdace-131">id</span></span>|<span data-ttu-id="cdace-132">String</span><span class="sxs-lookup"><span data-stu-id="cdace-132">String</span></span>|<span data-ttu-id="cdace-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cdace-133">Key of the entity.</span></span> <span data-ttu-id="cdace-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cdace-135">displayName</span></span>|<span data-ttu-id="cdace-136">String</span><span class="sxs-lookup"><span data-stu-id="cdace-136">String</span></span>|<span data-ttu-id="cdace-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cdace-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cdace-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-139">descrição</span><span class="sxs-lookup"><span data-stu-id="cdace-139">description</span></span>|<span data-ttu-id="cdace-140">String</span><span class="sxs-lookup"><span data-stu-id="cdace-140">String</span></span>|<span data-ttu-id="cdace-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdace-141">The description of the app.</span></span> <span data-ttu-id="cdace-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-143">publicador</span><span class="sxs-lookup"><span data-stu-id="cdace-143">publisher</span></span>|<span data-ttu-id="cdace-144">String</span><span class="sxs-lookup"><span data-stu-id="cdace-144">String</span></span>|<span data-ttu-id="cdace-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdace-145">The publisher of the app.</span></span> <span data-ttu-id="cdace-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cdace-147">largeIcon</span></span>|[<span data-ttu-id="cdace-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cdace-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cdace-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="cdace-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cdace-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cdace-151">createdDateTime</span></span>|<span data-ttu-id="cdace-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdace-152">DateTimeOffset</span></span>|<span data-ttu-id="cdace-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdace-153">The date and time the app was created.</span></span> <span data-ttu-id="cdace-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdace-155">lastModifiedDateTime</span></span>|<span data-ttu-id="cdace-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdace-156">DateTimeOffset</span></span>|<span data-ttu-id="cdace-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cdace-157">The date and time the app was last modified.</span></span> <span data-ttu-id="cdace-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cdace-159">isFeatured</span></span>|<span data-ttu-id="cdace-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdace-160">Boolean</span></span>|<span data-ttu-id="cdace-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cdace-162">privacyInformationUrl</span></span>|<span data-ttu-id="cdace-163">String</span><span class="sxs-lookup"><span data-stu-id="cdace-163">String</span></span>|<span data-ttu-id="cdace-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cdace-164">The privacy statement Url.</span></span> <span data-ttu-id="cdace-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cdace-166">informationUrl</span></span>|<span data-ttu-id="cdace-167">String</span><span class="sxs-lookup"><span data-stu-id="cdace-167">String</span></span>|<span data-ttu-id="cdace-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cdace-168">The more information Url.</span></span> <span data-ttu-id="cdace-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-170">owner</span><span class="sxs-lookup"><span data-stu-id="cdace-170">owner</span></span>|<span data-ttu-id="cdace-171">String</span><span class="sxs-lookup"><span data-stu-id="cdace-171">String</span></span>|<span data-ttu-id="cdace-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cdace-172">The owner of the app.</span></span> <span data-ttu-id="cdace-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-174">developer</span><span class="sxs-lookup"><span data-stu-id="cdace-174">developer</span></span>|<span data-ttu-id="cdace-175">String</span><span class="sxs-lookup"><span data-stu-id="cdace-175">String</span></span>|<span data-ttu-id="cdace-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdace-176">The developer of the app.</span></span> <span data-ttu-id="cdace-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-178">notes</span><span class="sxs-lookup"><span data-stu-id="cdace-178">notes</span></span>|<span data-ttu-id="cdace-179">String</span><span class="sxs-lookup"><span data-stu-id="cdace-179">String</span></span>|<span data-ttu-id="cdace-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdace-180">Notes for the app.</span></span> <span data-ttu-id="cdace-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdace-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="cdace-182">publishingState</span></span>|[<span data-ttu-id="cdace-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cdace-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cdace-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdace-184">The publishing state for the app.</span></span> <span data-ttu-id="cdace-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="cdace-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cdace-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdace-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cdace-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cdace-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cdace-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cdace-188">appAvailability</span></span>|[<span data-ttu-id="cdace-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="cdace-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="cdace-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdace-190">The Application's availability.</span></span> <span data-ttu-id="cdace-191">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdace-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="cdace-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="cdace-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cdace-193">version</span><span class="sxs-lookup"><span data-stu-id="cdace-193">version</span></span>|<span data-ttu-id="cdace-194">String</span><span class="sxs-lookup"><span data-stu-id="cdace-194">String</span></span>|<span data-ttu-id="cdace-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdace-195">The Application's version.</span></span> <span data-ttu-id="cdace-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cdace-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="cdace-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="cdace-197">bundleId</span></span>|<span data-ttu-id="cdace-198">String</span><span class="sxs-lookup"><span data-stu-id="cdace-198">String</span></span>|<span data-ttu-id="cdace-199">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="cdace-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="cdace-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cdace-200">appStoreUrl</span></span>|<span data-ttu-id="cdace-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdace-201">String</span></span>|<span data-ttu-id="cdace-202">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="cdace-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="cdace-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="cdace-203">applicableDeviceType</span></span>|[<span data-ttu-id="cdace-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="cdace-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="cdace-205">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="cdace-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="cdace-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cdace-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cdace-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cdace-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="cdace-208">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="cdace-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="cdace-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdace-209">Response</span></span>
<span data-ttu-id="cdace-210">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdace-210">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdace-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdace-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdace-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdace-212">Request</span></span>
<span data-ttu-id="cdace-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdace-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1104

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="cdace-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdace-214">Response</span></span>
<span data-ttu-id="cdace-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdace-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1276

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```



