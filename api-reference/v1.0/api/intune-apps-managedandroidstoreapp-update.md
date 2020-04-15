---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2ee86699e8dc1e714b38d8085bc25ebeb7bdcc2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446364"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="7ed39-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="7ed39-103">Update managedAndroidStoreApp</span></span>

<span data-ttu-id="7ed39-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ed39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ed39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ed39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ed39-106">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ed39-106">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ed39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ed39-107">Prerequisites</span></span>
<span data-ttu-id="7ed39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ed39-110">Permission type</span></span>|<span data-ttu-id="7ed39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ed39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ed39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ed39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ed39-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed39-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ed39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ed39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ed39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed39-115">Not supported.</span></span>|
|<span data-ttu-id="7ed39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ed39-116">Application</span></span>|<span data-ttu-id="7ed39-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ed39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ed39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7ed39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed39-119">Request headers</span></span>
|<span data-ttu-id="7ed39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ed39-120">Header</span></span>|<span data-ttu-id="7ed39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7ed39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ed39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ed39-122">Authorization</span></span>|<span data-ttu-id="7ed39-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ed39-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ed39-124">Accept</span></span>|<span data-ttu-id="7ed39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed39-126">Request body</span></span>
<span data-ttu-id="7ed39-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ed39-127">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="7ed39-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ed39-128">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="7ed39-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ed39-129">Property</span></span>|<span data-ttu-id="7ed39-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ed39-130">Type</span></span>|<span data-ttu-id="7ed39-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ed39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed39-132">id</span><span class="sxs-lookup"><span data-stu-id="7ed39-132">id</span></span>|<span data-ttu-id="7ed39-133">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-133">String</span></span>|<span data-ttu-id="7ed39-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7ed39-134">Key of the entity.</span></span> <span data-ttu-id="7ed39-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ed39-136">displayName</span></span>|<span data-ttu-id="7ed39-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed39-137">String</span></span>|<span data-ttu-id="7ed39-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7ed39-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7ed39-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-140">description</span><span class="sxs-lookup"><span data-stu-id="7ed39-140">description</span></span>|<span data-ttu-id="7ed39-141">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-141">String</span></span>|<span data-ttu-id="7ed39-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-142">The description of the app.</span></span> <span data-ttu-id="7ed39-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-144">publicador</span><span class="sxs-lookup"><span data-stu-id="7ed39-144">publisher</span></span>|<span data-ttu-id="7ed39-145">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-145">String</span></span>|<span data-ttu-id="7ed39-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-146">The publisher of the app.</span></span> <span data-ttu-id="7ed39-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7ed39-148">largeIcon</span></span>|[<span data-ttu-id="7ed39-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7ed39-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7ed39-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="7ed39-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7ed39-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed39-152">createdDateTime</span></span>|<span data-ttu-id="7ed39-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed39-153">DateTimeOffset</span></span>|<span data-ttu-id="7ed39-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-154">The date and time the app was created.</span></span> <span data-ttu-id="7ed39-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed39-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7ed39-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed39-157">DateTimeOffset</span></span>|<span data-ttu-id="7ed39-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7ed39-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7ed39-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7ed39-160">isFeatured</span></span>|<span data-ttu-id="7ed39-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ed39-161">Boolean</span></span>|<span data-ttu-id="7ed39-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7ed39-163">privacyInformationUrl</span></span>|<span data-ttu-id="7ed39-164">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-164">String</span></span>|<span data-ttu-id="7ed39-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7ed39-165">The privacy statement Url.</span></span> <span data-ttu-id="7ed39-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7ed39-167">informationUrl</span></span>|<span data-ttu-id="7ed39-168">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-168">String</span></span>|<span data-ttu-id="7ed39-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="7ed39-169">The more information Url.</span></span> <span data-ttu-id="7ed39-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-171">owner</span><span class="sxs-lookup"><span data-stu-id="7ed39-171">owner</span></span>|<span data-ttu-id="7ed39-172">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-172">String</span></span>|<span data-ttu-id="7ed39-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-173">The owner of the app.</span></span> <span data-ttu-id="7ed39-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-175">developer</span><span class="sxs-lookup"><span data-stu-id="7ed39-175">developer</span></span>|<span data-ttu-id="7ed39-176">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-176">String</span></span>|<span data-ttu-id="7ed39-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-177">The developer of the app.</span></span> <span data-ttu-id="7ed39-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-179">notes</span><span class="sxs-lookup"><span data-stu-id="7ed39-179">notes</span></span>|<span data-ttu-id="7ed39-180">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-180">String</span></span>|<span data-ttu-id="7ed39-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-181">Notes for the app.</span></span> <span data-ttu-id="7ed39-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed39-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="7ed39-183">publishingState</span></span>|[<span data-ttu-id="7ed39-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7ed39-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7ed39-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-185">The publishing state for the app.</span></span> <span data-ttu-id="7ed39-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="7ed39-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7ed39-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ed39-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7ed39-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7ed39-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7ed39-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="7ed39-189">appAvailability</span></span>|[<span data-ttu-id="7ed39-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="7ed39-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="7ed39-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-191">The Application's availability.</span></span> <span data-ttu-id="7ed39-192">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ed39-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="7ed39-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="7ed39-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="7ed39-194">version</span><span class="sxs-lookup"><span data-stu-id="7ed39-194">version</span></span>|<span data-ttu-id="7ed39-195">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-195">String</span></span>|<span data-ttu-id="7ed39-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-196">The Application's version.</span></span> <span data-ttu-id="7ed39-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed39-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="7ed39-198">packageId</span><span class="sxs-lookup"><span data-stu-id="7ed39-198">packageId</span></span>|<span data-ttu-id="7ed39-199">String</span><span class="sxs-lookup"><span data-stu-id="7ed39-199">String</span></span>|<span data-ttu-id="7ed39-200">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed39-200">The app's package ID.</span></span>|
|<span data-ttu-id="7ed39-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7ed39-201">appStoreUrl</span></span>|<span data-ttu-id="7ed39-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed39-202">String</span></span>|<span data-ttu-id="7ed39-203">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="7ed39-203">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="7ed39-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ed39-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7ed39-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ed39-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="7ed39-206">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed39-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="7ed39-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed39-207">Response</span></span>
<span data-ttu-id="7ed39-208">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ed39-208">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed39-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ed39-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ed39-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed39-210">Request</span></span>
<span data-ttu-id="7ed39-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ed39-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ed39-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed39-212">Response</span></span>
<span data-ttu-id="7ed39-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ed39-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






