---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
author: tfitzmac
ms.openlocfilehash: c592238c7c48939b47dfc772a93dea4f07f7bf06
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327640"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="4d047-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="4d047-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="4d047-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d047-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d047-105">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d047-105">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d047-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d047-106">Prerequisites</span></span>
<span data-ttu-id="4d047-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d047-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d047-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d047-109">Permission type</span></span>|<span data-ttu-id="4d047-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d047-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d047-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d047-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d047-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d047-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4d047-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d047-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d047-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d047-114">Not supported.</span></span>|
|<span data-ttu-id="4d047-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d047-115">Application</span></span>|<span data-ttu-id="4d047-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d047-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d047-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d047-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="4d047-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d047-118">Request headers</span></span>
|<span data-ttu-id="4d047-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d047-119">Header</span></span>|<span data-ttu-id="4d047-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4d047-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d047-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d047-121">Authorization</span></span>|<span data-ttu-id="4d047-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d047-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d047-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4d047-123">Accept</span></span>|<span data-ttu-id="4d047-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d047-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d047-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d047-125">Request body</span></span>
<span data-ttu-id="4d047-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d047-126">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="4d047-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d047-127">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="4d047-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d047-128">Property</span></span>|<span data-ttu-id="4d047-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d047-129">Type</span></span>|<span data-ttu-id="4d047-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d047-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d047-131">id</span><span class="sxs-lookup"><span data-stu-id="4d047-131">id</span></span>|<span data-ttu-id="4d047-132">String</span><span class="sxs-lookup"><span data-stu-id="4d047-132">String</span></span>|<span data-ttu-id="4d047-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4d047-133">Key of the entity.</span></span> <span data-ttu-id="4d047-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4d047-135">displayName</span></span>|<span data-ttu-id="4d047-136">String</span><span class="sxs-lookup"><span data-stu-id="4d047-136">String</span></span>|<span data-ttu-id="4d047-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4d047-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4d047-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-139">description</span><span class="sxs-lookup"><span data-stu-id="4d047-139">description</span></span>|<span data-ttu-id="4d047-140">String</span><span class="sxs-lookup"><span data-stu-id="4d047-140">String</span></span>|<span data-ttu-id="4d047-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-141">The description of the app.</span></span> <span data-ttu-id="4d047-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-143">publisher</span><span class="sxs-lookup"><span data-stu-id="4d047-143">publisher</span></span>|<span data-ttu-id="4d047-144">String</span><span class="sxs-lookup"><span data-stu-id="4d047-144">String</span></span>|<span data-ttu-id="4d047-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-145">The publisher of the app.</span></span> <span data-ttu-id="4d047-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4d047-147">largeIcon</span></span>|[<span data-ttu-id="4d047-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4d047-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4d047-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4d047-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4d047-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d047-151">createdDateTime</span></span>|<span data-ttu-id="4d047-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d047-152">DateTimeOffset</span></span>|<span data-ttu-id="4d047-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-153">The date and time the app was created.</span></span> <span data-ttu-id="4d047-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d047-155">lastModifiedDateTime</span></span>|<span data-ttu-id="4d047-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d047-156">DateTimeOffset</span></span>|<span data-ttu-id="4d047-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4d047-157">The date and time the app was last modified.</span></span> <span data-ttu-id="4d047-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4d047-159">isFeatured</span></span>|<span data-ttu-id="4d047-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d047-160">Boolean</span></span>|<span data-ttu-id="4d047-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4d047-162">privacyInformationUrl</span></span>|<span data-ttu-id="4d047-163">String</span><span class="sxs-lookup"><span data-stu-id="4d047-163">String</span></span>|<span data-ttu-id="4d047-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4d047-164">The privacy statement Url.</span></span> <span data-ttu-id="4d047-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4d047-166">informationUrl</span></span>|<span data-ttu-id="4d047-167">String</span><span class="sxs-lookup"><span data-stu-id="4d047-167">String</span></span>|<span data-ttu-id="4d047-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4d047-168">The more information Url.</span></span> <span data-ttu-id="4d047-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-170">owner</span><span class="sxs-lookup"><span data-stu-id="4d047-170">owner</span></span>|<span data-ttu-id="4d047-171">String</span><span class="sxs-lookup"><span data-stu-id="4d047-171">String</span></span>|<span data-ttu-id="4d047-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4d047-172">The owner of the app.</span></span> <span data-ttu-id="4d047-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-174">developer</span><span class="sxs-lookup"><span data-stu-id="4d047-174">developer</span></span>|<span data-ttu-id="4d047-175">String</span><span class="sxs-lookup"><span data-stu-id="4d047-175">String</span></span>|<span data-ttu-id="4d047-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-176">The developer of the app.</span></span> <span data-ttu-id="4d047-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-178">Observações</span><span class="sxs-lookup"><span data-stu-id="4d047-178">notes</span></span>|<span data-ttu-id="4d047-179">String</span><span class="sxs-lookup"><span data-stu-id="4d047-179">String</span></span>|<span data-ttu-id="4d047-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-180">Notes for the app.</span></span> <span data-ttu-id="4d047-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4d047-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="4d047-182">publishingState</span></span>|[<span data-ttu-id="4d047-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4d047-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4d047-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-184">The publishing state for the app.</span></span> <span data-ttu-id="4d047-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4d047-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4d047-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d047-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4d047-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4d047-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4d047-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4d047-188">appAvailability</span></span>|[<span data-ttu-id="4d047-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4d047-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4d047-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-190">The Application's availability.</span></span> <span data-ttu-id="4d047-191">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d047-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4d047-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4d047-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4d047-193">version</span><span class="sxs-lookup"><span data-stu-id="4d047-193">version</span></span>|<span data-ttu-id="4d047-194">String</span><span class="sxs-lookup"><span data-stu-id="4d047-194">String</span></span>|<span data-ttu-id="4d047-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-195">The Application's version.</span></span> <span data-ttu-id="4d047-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d047-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4d047-197">packageId</span><span class="sxs-lookup"><span data-stu-id="4d047-197">packageId</span></span>|<span data-ttu-id="4d047-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d047-198">String</span></span>|<span data-ttu-id="4d047-199">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d047-199">The app's package ID.</span></span>|
|<span data-ttu-id="4d047-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4d047-200">appStoreUrl</span></span>|<span data-ttu-id="4d047-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d047-201">String</span></span>|<span data-ttu-id="4d047-202">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="4d047-202">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="4d047-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4d047-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4d047-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4d047-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="4d047-205">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="4d047-205">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="4d047-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d047-206">Response</span></span>
<span data-ttu-id="4d047-207">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d047-207">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d047-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d047-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d047-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d047-209">Request</span></span>
<span data-ttu-id="4d047-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d047-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d047-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d047-211">Response</span></span>
<span data-ttu-id="4d047-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d047-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



