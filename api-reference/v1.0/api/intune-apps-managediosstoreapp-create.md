---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
author: tfitzmac
ms.openlocfilehash: 392d7fee5685afe1804c8832bdd1fcb72ff6d3a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319464"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="9fd5e-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="9fd5e-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="9fd5e-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fd5e-105">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fd5e-105">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fd5e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fd5e-106">Prerequisites</span></span>
<span data-ttu-id="9fd5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fd5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fd5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fd5e-109">Permission type</span></span>|<span data-ttu-id="9fd5e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fd5e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9fd5e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd5e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fd5e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fd5e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-114">Not supported.</span></span>|
|<span data-ttu-id="9fd5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fd5e-115">Application</span></span>|<span data-ttu-id="9fd5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fd5e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd5e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9fd5e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd5e-118">Request headers</span></span>
|<span data-ttu-id="9fd5e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fd5e-119">Header</span></span>|<span data-ttu-id="9fd5e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9fd5e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fd5e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fd5e-121">Authorization</span></span>|<span data-ttu-id="9fd5e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fd5e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9fd5e-123">Accept</span></span>|<span data-ttu-id="9fd5e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9fd5e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fd5e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd5e-125">Request body</span></span>
<span data-ttu-id="9fd5e-126">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-126">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="9fd5e-127">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-127">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="9fd5e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fd5e-128">Property</span></span>|<span data-ttu-id="9fd5e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fd5e-129">Type</span></span>|<span data-ttu-id="9fd5e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd5e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fd5e-131">id</span><span class="sxs-lookup"><span data-stu-id="9fd5e-131">id</span></span>|<span data-ttu-id="9fd5e-132">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-132">String</span></span>|<span data-ttu-id="9fd5e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-133">Key of the entity.</span></span> <span data-ttu-id="9fd5e-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9fd5e-135">displayName</span></span>|<span data-ttu-id="9fd5e-136">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-136">String</span></span>|<span data-ttu-id="9fd5e-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9fd5e-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-139">description</span><span class="sxs-lookup"><span data-stu-id="9fd5e-139">description</span></span>|<span data-ttu-id="9fd5e-140">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-140">String</span></span>|<span data-ttu-id="9fd5e-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-141">The description of the app.</span></span> <span data-ttu-id="9fd5e-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-143">publisher</span><span class="sxs-lookup"><span data-stu-id="9fd5e-143">publisher</span></span>|<span data-ttu-id="9fd5e-144">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-144">String</span></span>|<span data-ttu-id="9fd5e-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-145">The publisher of the app.</span></span> <span data-ttu-id="9fd5e-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9fd5e-147">largeIcon</span></span>|[<span data-ttu-id="9fd5e-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9fd5e-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9fd5e-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9fd5e-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fd5e-151">createdDateTime</span></span>|<span data-ttu-id="9fd5e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fd5e-152">DateTimeOffset</span></span>|<span data-ttu-id="9fd5e-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-153">The date and time the app was created.</span></span> <span data-ttu-id="9fd5e-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fd5e-155">lastModifiedDateTime</span></span>|<span data-ttu-id="9fd5e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fd5e-156">DateTimeOffset</span></span>|<span data-ttu-id="9fd5e-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-157">The date and time the app was last modified.</span></span> <span data-ttu-id="9fd5e-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9fd5e-159">isFeatured</span></span>|<span data-ttu-id="9fd5e-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fd5e-160">Boolean</span></span>|<span data-ttu-id="9fd5e-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9fd5e-162">privacyInformationUrl</span></span>|<span data-ttu-id="9fd5e-163">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-163">String</span></span>|<span data-ttu-id="9fd5e-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-164">The privacy statement Url.</span></span> <span data-ttu-id="9fd5e-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9fd5e-166">informationUrl</span></span>|<span data-ttu-id="9fd5e-167">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-167">String</span></span>|<span data-ttu-id="9fd5e-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-168">The more information Url.</span></span> <span data-ttu-id="9fd5e-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-170">owner</span><span class="sxs-lookup"><span data-stu-id="9fd5e-170">owner</span></span>|<span data-ttu-id="9fd5e-171">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-171">String</span></span>|<span data-ttu-id="9fd5e-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-172">The owner of the app.</span></span> <span data-ttu-id="9fd5e-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-174">developer</span><span class="sxs-lookup"><span data-stu-id="9fd5e-174">developer</span></span>|<span data-ttu-id="9fd5e-175">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-175">String</span></span>|<span data-ttu-id="9fd5e-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-176">The developer of the app.</span></span> <span data-ttu-id="9fd5e-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-178">Observações</span><span class="sxs-lookup"><span data-stu-id="9fd5e-178">notes</span></span>|<span data-ttu-id="9fd5e-179">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-179">String</span></span>|<span data-ttu-id="9fd5e-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-180">Notes for the app.</span></span> <span data-ttu-id="9fd5e-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fd5e-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="9fd5e-182">publishingState</span></span>|[<span data-ttu-id="9fd5e-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9fd5e-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9fd5e-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-184">The publishing state for the app.</span></span> <span data-ttu-id="9fd5e-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9fd5e-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fd5e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9fd5e-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9fd5e-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9fd5e-188">appAvailability</span></span>|[<span data-ttu-id="9fd5e-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="9fd5e-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="9fd5e-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-190">The Application's availability.</span></span> <span data-ttu-id="9fd5e-191">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fd5e-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="9fd5e-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="9fd5e-193">version</span><span class="sxs-lookup"><span data-stu-id="9fd5e-193">version</span></span>|<span data-ttu-id="9fd5e-194">String</span><span class="sxs-lookup"><span data-stu-id="9fd5e-194">String</span></span>|<span data-ttu-id="9fd5e-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-195">The Application's version.</span></span> <span data-ttu-id="9fd5e-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fd5e-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="9fd5e-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="9fd5e-197">bundleId</span></span>|<span data-ttu-id="9fd5e-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fd5e-198">String</span></span>|<span data-ttu-id="9fd5e-199">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="9fd5e-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9fd5e-200">appStoreUrl</span></span>|<span data-ttu-id="9fd5e-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fd5e-201">String</span></span>|<span data-ttu-id="9fd5e-202">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="9fd5e-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9fd5e-203">applicableDeviceType</span></span>|[<span data-ttu-id="9fd5e-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9fd5e-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9fd5e-205">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9fd5e-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9fd5e-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9fd5e-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9fd5e-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9fd5e-208">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="9fd5e-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd5e-209">Response</span></span>
<span data-ttu-id="9fd5e-210">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-210">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fd5e-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fd5e-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fd5e-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd5e-212">Request</span></span>
<span data-ttu-id="9fd5e-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1084

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
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="9fd5e-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd5e-214">Response</span></span>
<span data-ttu-id="9fd5e-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fd5e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1256

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
    "v12_0": true
  }
}
```



