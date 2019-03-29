---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a540d5a0acb2cc6db792c4b52a1a0eeb93623028
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970909"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="9ca28-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="9ca28-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="9ca28-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ca28-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ca28-105">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ca28-105">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ca28-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ca28-106">Prerequisites</span></span>
<span data-ttu-id="9ca28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ca28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ca28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ca28-109">Permission type</span></span>|<span data-ttu-id="9ca28-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ca28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ca28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ca28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ca28-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ca28-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ca28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ca28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ca28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ca28-114">Not supported.</span></span>|
|<span data-ttu-id="9ca28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ca28-115">Application</span></span>|<span data-ttu-id="9ca28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ca28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ca28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ca28-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9ca28-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ca28-118">Request headers</span></span>
|<span data-ttu-id="9ca28-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ca28-119">Header</span></span>|<span data-ttu-id="9ca28-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9ca28-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ca28-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ca28-121">Authorization</span></span>|<span data-ttu-id="9ca28-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ca28-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ca28-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ca28-123">Accept</span></span>|<span data-ttu-id="9ca28-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9ca28-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ca28-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ca28-125">Request body</span></span>
<span data-ttu-id="9ca28-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ca28-126">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="9ca28-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ca28-127">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="9ca28-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ca28-128">Property</span></span>|<span data-ttu-id="9ca28-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ca28-129">Type</span></span>|<span data-ttu-id="9ca28-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ca28-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ca28-131">id</span><span class="sxs-lookup"><span data-stu-id="9ca28-131">id</span></span>|<span data-ttu-id="9ca28-132">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-132">String</span></span>|<span data-ttu-id="9ca28-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ca28-133">Key of the entity.</span></span> <span data-ttu-id="9ca28-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9ca28-135">displayName</span></span>|<span data-ttu-id="9ca28-136">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-136">String</span></span>|<span data-ttu-id="9ca28-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9ca28-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9ca28-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-139">descrição</span><span class="sxs-lookup"><span data-stu-id="9ca28-139">description</span></span>|<span data-ttu-id="9ca28-140">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-140">String</span></span>|<span data-ttu-id="9ca28-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-141">The description of the app.</span></span> <span data-ttu-id="9ca28-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-143">publicador</span><span class="sxs-lookup"><span data-stu-id="9ca28-143">publisher</span></span>|<span data-ttu-id="9ca28-144">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-144">String</span></span>|<span data-ttu-id="9ca28-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-145">The publisher of the app.</span></span> <span data-ttu-id="9ca28-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ca28-147">largeIcon</span></span>|[<span data-ttu-id="9ca28-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ca28-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ca28-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9ca28-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9ca28-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ca28-151">createdDateTime</span></span>|<span data-ttu-id="9ca28-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ca28-152">DateTimeOffset</span></span>|<span data-ttu-id="9ca28-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-153">The date and time the app was created.</span></span> <span data-ttu-id="9ca28-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ca28-155">lastModifiedDateTime</span></span>|<span data-ttu-id="9ca28-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ca28-156">DateTimeOffset</span></span>|<span data-ttu-id="9ca28-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9ca28-157">The date and time the app was last modified.</span></span> <span data-ttu-id="9ca28-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ca28-159">isFeatured</span></span>|<span data-ttu-id="9ca28-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ca28-160">Boolean</span></span>|<span data-ttu-id="9ca28-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ca28-162">privacyInformationUrl</span></span>|<span data-ttu-id="9ca28-163">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-163">String</span></span>|<span data-ttu-id="9ca28-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9ca28-164">The privacy statement Url.</span></span> <span data-ttu-id="9ca28-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ca28-166">informationUrl</span></span>|<span data-ttu-id="9ca28-167">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-167">String</span></span>|<span data-ttu-id="9ca28-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9ca28-168">The more information Url.</span></span> <span data-ttu-id="9ca28-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-170">owner</span><span class="sxs-lookup"><span data-stu-id="9ca28-170">owner</span></span>|<span data-ttu-id="9ca28-171">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-171">String</span></span>|<span data-ttu-id="9ca28-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-172">The owner of the app.</span></span> <span data-ttu-id="9ca28-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-174">developer</span><span class="sxs-lookup"><span data-stu-id="9ca28-174">developer</span></span>|<span data-ttu-id="9ca28-175">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-175">String</span></span>|<span data-ttu-id="9ca28-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-176">The developer of the app.</span></span> <span data-ttu-id="9ca28-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-178">notes</span><span class="sxs-lookup"><span data-stu-id="9ca28-178">notes</span></span>|<span data-ttu-id="9ca28-179">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-179">String</span></span>|<span data-ttu-id="9ca28-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-180">Notes for the app.</span></span> <span data-ttu-id="9ca28-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ca28-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ca28-182">publishingState</span></span>|[<span data-ttu-id="9ca28-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9ca28-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9ca28-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-184">The publishing state for the app.</span></span> <span data-ttu-id="9ca28-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9ca28-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ca28-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ca28-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9ca28-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9ca28-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9ca28-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9ca28-188">appAvailability</span></span>|[<span data-ttu-id="9ca28-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="9ca28-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="9ca28-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-190">The Application's availability.</span></span> <span data-ttu-id="9ca28-191">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ca28-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="9ca28-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9ca28-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="9ca28-193">version</span><span class="sxs-lookup"><span data-stu-id="9ca28-193">version</span></span>|<span data-ttu-id="9ca28-194">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-194">String</span></span>|<span data-ttu-id="9ca28-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-195">The Application's version.</span></span> <span data-ttu-id="9ca28-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ca28-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="9ca28-197">packageId</span><span class="sxs-lookup"><span data-stu-id="9ca28-197">packageId</span></span>|<span data-ttu-id="9ca28-198">String</span><span class="sxs-lookup"><span data-stu-id="9ca28-198">String</span></span>|<span data-ttu-id="9ca28-199">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ca28-199">The app's package ID.</span></span>|
|<span data-ttu-id="9ca28-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9ca28-200">appStoreUrl</span></span>|<span data-ttu-id="9ca28-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ca28-201">String</span></span>|<span data-ttu-id="9ca28-202">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="9ca28-202">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="9ca28-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ca28-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9ca28-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ca28-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="9ca28-205">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="9ca28-205">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="9ca28-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ca28-206">Response</span></span>
<span data-ttu-id="9ca28-207">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ca28-207">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ca28-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ca28-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ca28-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ca28-209">Request</span></span>
<span data-ttu-id="9ca28-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ca28-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ca28-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ca28-211">Response</span></span>
<span data-ttu-id="9ca28-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ca28-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



