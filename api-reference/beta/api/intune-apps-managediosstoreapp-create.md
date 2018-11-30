---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
ms.openlocfilehash: 5b1d9a0292e457dc7be5ec97802b4dc8bbefb6a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038430"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="84796-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="84796-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="84796-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="84796-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84796-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="84796-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84796-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="84796-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84796-107">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="84796-107">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84796-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84796-108">Prerequisites</span></span>
<span data-ttu-id="84796-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84796-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84796-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84796-111">Permission type</span></span>|<span data-ttu-id="84796-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84796-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84796-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84796-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84796-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84796-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84796-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84796-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84796-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84796-116">Not supported.</span></span>|
|<span data-ttu-id="84796-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84796-117">Application</span></span>|<span data-ttu-id="84796-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84796-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84796-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84796-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="84796-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84796-120">Request headers</span></span>
|<span data-ttu-id="84796-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84796-121">Header</span></span>|<span data-ttu-id="84796-122">Valor</span><span class="sxs-lookup"><span data-stu-id="84796-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84796-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84796-123">Authorization</span></span>|<span data-ttu-id="84796-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84796-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84796-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84796-125">Accept</span></span>|<span data-ttu-id="84796-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84796-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84796-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84796-127">Request body</span></span>
<span data-ttu-id="84796-128">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="84796-128">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="84796-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="84796-129">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="84796-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84796-130">Property</span></span>|<span data-ttu-id="84796-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="84796-131">Type</span></span>|<span data-ttu-id="84796-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="84796-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84796-133">id</span><span class="sxs-lookup"><span data-stu-id="84796-133">id</span></span>|<span data-ttu-id="84796-134">String</span><span class="sxs-lookup"><span data-stu-id="84796-134">String</span></span>|<span data-ttu-id="84796-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="84796-135">Key of the entity.</span></span> <span data-ttu-id="84796-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-137">displayName</span><span class="sxs-lookup"><span data-stu-id="84796-137">displayName</span></span>|<span data-ttu-id="84796-138">String</span><span class="sxs-lookup"><span data-stu-id="84796-138">String</span></span>|<span data-ttu-id="84796-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="84796-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="84796-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-141">description</span><span class="sxs-lookup"><span data-stu-id="84796-141">description</span></span>|<span data-ttu-id="84796-142">String</span><span class="sxs-lookup"><span data-stu-id="84796-142">String</span></span>|<span data-ttu-id="84796-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84796-143">The description of the app.</span></span> <span data-ttu-id="84796-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-145">publisher</span><span class="sxs-lookup"><span data-stu-id="84796-145">publisher</span></span>|<span data-ttu-id="84796-146">String</span><span class="sxs-lookup"><span data-stu-id="84796-146">String</span></span>|<span data-ttu-id="84796-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84796-147">The publisher of the app.</span></span> <span data-ttu-id="84796-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="84796-149">largeIcon</span></span>|[<span data-ttu-id="84796-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="84796-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="84796-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="84796-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="84796-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84796-153">createdDateTime</span></span>|<span data-ttu-id="84796-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84796-154">DateTimeOffset</span></span>|<span data-ttu-id="84796-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84796-155">The date and time the app was created.</span></span> <span data-ttu-id="84796-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84796-157">lastModifiedDateTime</span></span>|<span data-ttu-id="84796-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84796-158">DateTimeOffset</span></span>|<span data-ttu-id="84796-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="84796-159">The date and time the app was last modified.</span></span> <span data-ttu-id="84796-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="84796-161">isFeatured</span></span>|<span data-ttu-id="84796-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="84796-162">Boolean</span></span>|<span data-ttu-id="84796-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="84796-164">privacyInformationUrl</span></span>|<span data-ttu-id="84796-165">String</span><span class="sxs-lookup"><span data-stu-id="84796-165">String</span></span>|<span data-ttu-id="84796-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="84796-166">The privacy statement Url.</span></span> <span data-ttu-id="84796-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="84796-168">informationUrl</span></span>|<span data-ttu-id="84796-169">String</span><span class="sxs-lookup"><span data-stu-id="84796-169">String</span></span>|<span data-ttu-id="84796-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="84796-170">The more information Url.</span></span> <span data-ttu-id="84796-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-172">owner</span><span class="sxs-lookup"><span data-stu-id="84796-172">owner</span></span>|<span data-ttu-id="84796-173">String</span><span class="sxs-lookup"><span data-stu-id="84796-173">String</span></span>|<span data-ttu-id="84796-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="84796-174">The owner of the app.</span></span> <span data-ttu-id="84796-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-176">developer</span><span class="sxs-lookup"><span data-stu-id="84796-176">developer</span></span>|<span data-ttu-id="84796-177">String</span><span class="sxs-lookup"><span data-stu-id="84796-177">String</span></span>|<span data-ttu-id="84796-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84796-178">The developer of the app.</span></span> <span data-ttu-id="84796-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-180">Observações</span><span class="sxs-lookup"><span data-stu-id="84796-180">notes</span></span>|<span data-ttu-id="84796-181">String</span><span class="sxs-lookup"><span data-stu-id="84796-181">String</span></span>|<span data-ttu-id="84796-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84796-182">Notes for the app.</span></span> <span data-ttu-id="84796-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="84796-184">uploadState</span></span>|<span data-ttu-id="84796-185">Int32</span><span class="sxs-lookup"><span data-stu-id="84796-185">Int32</span></span>|<span data-ttu-id="84796-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="84796-186">The upload state.</span></span> <span data-ttu-id="84796-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84796-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="84796-188">publishingState</span></span>|[<span data-ttu-id="84796-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="84796-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="84796-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84796-190">The publishing state for the app.</span></span> <span data-ttu-id="84796-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="84796-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="84796-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84796-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="84796-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="84796-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="84796-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="84796-194">appAvailability</span></span>|[<span data-ttu-id="84796-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="84796-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="84796-196">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84796-196">The Application's availability.</span></span> <span data-ttu-id="84796-197">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="84796-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="84796-198">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="84796-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="84796-199">version</span><span class="sxs-lookup"><span data-stu-id="84796-199">version</span></span>|<span data-ttu-id="84796-200">String</span><span class="sxs-lookup"><span data-stu-id="84796-200">String</span></span>|<span data-ttu-id="84796-201">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84796-201">The Application's version.</span></span> <span data-ttu-id="84796-202">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="84796-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="84796-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="84796-203">bundleId</span></span>|<span data-ttu-id="84796-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84796-204">String</span></span>|<span data-ttu-id="84796-205">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="84796-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="84796-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="84796-206">appStoreUrl</span></span>|<span data-ttu-id="84796-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84796-207">String</span></span>|<span data-ttu-id="84796-208">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="84796-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="84796-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="84796-209">applicableDeviceType</span></span>|[<span data-ttu-id="84796-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="84796-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="84796-211">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="84796-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="84796-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="84796-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="84796-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="84796-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="84796-214">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="84796-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="84796-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="84796-215">Response</span></span>
<span data-ttu-id="84796-216">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84796-216">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84796-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84796-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="84796-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84796-218">Request</span></span>
<span data-ttu-id="84796-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84796-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1170

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
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
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="84796-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="84796-220">Response</span></span>
<span data-ttu-id="84796-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84796-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1278

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
  "uploadState": 11,
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
    "v12_0": true
  }
}
```





