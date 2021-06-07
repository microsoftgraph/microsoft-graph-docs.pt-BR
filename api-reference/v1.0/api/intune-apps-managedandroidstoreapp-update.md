---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f0d76b4960a336e5bddb1c60887b18b64328dbd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754277"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="18a3e-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="18a3e-103">Update managedAndroidStoreApp</span></span>

<span data-ttu-id="18a3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18a3e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18a3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a3e-106">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="18a3e-106">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18a3e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18a3e-107">Prerequisites</span></span>
<span data-ttu-id="18a3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18a3e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18a3e-110">Permission type</span></span>|<span data-ttu-id="18a3e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18a3e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18a3e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18a3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18a3e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a3e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18a3e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18a3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18a3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18a3e-115">Not supported.</span></span>|
|<span data-ttu-id="18a3e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18a3e-116">Application</span></span>|<span data-ttu-id="18a3e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a3e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18a3e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18a3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="18a3e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18a3e-119">Request headers</span></span>
|<span data-ttu-id="18a3e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18a3e-120">Header</span></span>|<span data-ttu-id="18a3e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="18a3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18a3e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18a3e-122">Authorization</span></span>|<span data-ttu-id="18a3e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18a3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18a3e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18a3e-124">Accept</span></span>|<span data-ttu-id="18a3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18a3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18a3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18a3e-126">Request body</span></span>
<span data-ttu-id="18a3e-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="18a3e-127">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="18a3e-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="18a3e-128">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="18a3e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18a3e-129">Property</span></span>|<span data-ttu-id="18a3e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a3e-130">Type</span></span>|<span data-ttu-id="18a3e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18a3e-132">id</span><span class="sxs-lookup"><span data-stu-id="18a3e-132">id</span></span>|<span data-ttu-id="18a3e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a3e-133">String</span></span>|<span data-ttu-id="18a3e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18a3e-134">Key of the entity.</span></span> <span data-ttu-id="18a3e-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="18a3e-136">displayName</span></span>|<span data-ttu-id="18a3e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a3e-137">String</span></span>|<span data-ttu-id="18a3e-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="18a3e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="18a3e-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-140">descrição</span><span class="sxs-lookup"><span data-stu-id="18a3e-140">description</span></span>|<span data-ttu-id="18a3e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a3e-141">String</span></span>|<span data-ttu-id="18a3e-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-142">The description of the app.</span></span> <span data-ttu-id="18a3e-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-144">publicador</span><span class="sxs-lookup"><span data-stu-id="18a3e-144">publisher</span></span>|<span data-ttu-id="18a3e-145">String</span><span class="sxs-lookup"><span data-stu-id="18a3e-145">String</span></span>|<span data-ttu-id="18a3e-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-146">The publisher of the app.</span></span> <span data-ttu-id="18a3e-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="18a3e-148">largeIcon</span></span>|[<span data-ttu-id="18a3e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18a3e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18a3e-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="18a3e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="18a3e-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18a3e-152">createdDateTime</span></span>|<span data-ttu-id="18a3e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a3e-153">DateTimeOffset</span></span>|<span data-ttu-id="18a3e-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-154">The date and time the app was created.</span></span> <span data-ttu-id="18a3e-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18a3e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="18a3e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a3e-157">DateTimeOffset</span></span>|<span data-ttu-id="18a3e-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="18a3e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="18a3e-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="18a3e-160">isFeatured</span></span>|<span data-ttu-id="18a3e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="18a3e-161">Boolean</span></span>|<span data-ttu-id="18a3e-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18a3e-163">privacyInformationUrl</span></span>|<span data-ttu-id="18a3e-164">String</span><span class="sxs-lookup"><span data-stu-id="18a3e-164">String</span></span>|<span data-ttu-id="18a3e-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="18a3e-165">The privacy statement Url.</span></span> <span data-ttu-id="18a3e-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18a3e-167">informationUrl</span></span>|<span data-ttu-id="18a3e-168">String</span><span class="sxs-lookup"><span data-stu-id="18a3e-168">String</span></span>|<span data-ttu-id="18a3e-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="18a3e-169">The more information Url.</span></span> <span data-ttu-id="18a3e-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="18a3e-171">owner</span></span>|<span data-ttu-id="18a3e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a3e-172">String</span></span>|<span data-ttu-id="18a3e-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-173">The owner of the app.</span></span> <span data-ttu-id="18a3e-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-175">developer</span><span class="sxs-lookup"><span data-stu-id="18a3e-175">developer</span></span>|<span data-ttu-id="18a3e-176">String</span><span class="sxs-lookup"><span data-stu-id="18a3e-176">String</span></span>|<span data-ttu-id="18a3e-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-177">The developer of the app.</span></span> <span data-ttu-id="18a3e-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-179">notes</span><span class="sxs-lookup"><span data-stu-id="18a3e-179">notes</span></span>|<span data-ttu-id="18a3e-180">String</span><span class="sxs-lookup"><span data-stu-id="18a3e-180">String</span></span>|<span data-ttu-id="18a3e-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-181">Notes for the app.</span></span> <span data-ttu-id="18a3e-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a3e-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="18a3e-183">publishingState</span></span>|[<span data-ttu-id="18a3e-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="18a3e-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="18a3e-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-185">The publishing state for the app.</span></span> <span data-ttu-id="18a3e-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="18a3e-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="18a3e-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18a3e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="18a3e-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="18a3e-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="18a3e-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="18a3e-189">appAvailability</span></span>|[<span data-ttu-id="18a3e-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="18a3e-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="18a3e-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-191">The Application's availability.</span></span> <span data-ttu-id="18a3e-192">Herdado [de managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="18a3e-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="18a3e-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="18a3e-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="18a3e-194">version</span><span class="sxs-lookup"><span data-stu-id="18a3e-194">version</span></span>|<span data-ttu-id="18a3e-195">String</span><span class="sxs-lookup"><span data-stu-id="18a3e-195">String</span></span>|<span data-ttu-id="18a3e-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-196">The Application's version.</span></span> <span data-ttu-id="18a3e-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a3e-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="18a3e-198">packageId</span><span class="sxs-lookup"><span data-stu-id="18a3e-198">packageId</span></span>|<span data-ttu-id="18a3e-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a3e-199">String</span></span>|<span data-ttu-id="18a3e-200">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a3e-200">The app's package ID.</span></span>|
|<span data-ttu-id="18a3e-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="18a3e-201">appStoreUrl</span></span>|<span data-ttu-id="18a3e-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a3e-202">String</span></span>|<span data-ttu-id="18a3e-203">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="18a3e-203">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="18a3e-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18a3e-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="18a3e-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18a3e-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="18a3e-206">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="18a3e-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="18a3e-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a3e-207">Response</span></span>
<span data-ttu-id="18a3e-208">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18a3e-208">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18a3e-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18a3e-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="18a3e-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18a3e-210">Request</span></span>
<span data-ttu-id="18a3e-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18a3e-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1056

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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="18a3e-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a3e-212">Response</span></span>
<span data-ttu-id="18a3e-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18a3e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1228

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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  }
}
```




