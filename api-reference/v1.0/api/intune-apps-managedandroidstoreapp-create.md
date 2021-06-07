---
title: Criar managedAndroidStoreApp
description: Cria um novo objeto managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8104dbc8259352d917f8b05761d06aa3f3dea805
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754305"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="a8bc9-103">Criar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="a8bc9-103">Create managedAndroidStoreApp</span></span>

<span data-ttu-id="a8bc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8bc9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8bc9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8bc9-106">Cria um novo objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a8bc9-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8bc9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8bc9-107">Prerequisites</span></span>
<span data-ttu-id="a8bc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8bc9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8bc9-110">Permission type</span></span>|<span data-ttu-id="a8bc9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8bc9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8bc9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8bc9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8bc9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8bc9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-115">Not supported.</span></span>|
|<span data-ttu-id="a8bc9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8bc9-116">Application</span></span>|<span data-ttu-id="a8bc9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8bc9-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8bc9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8bc9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a8bc9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8bc9-119">Request headers</span></span>
|<span data-ttu-id="a8bc9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8bc9-120">Header</span></span>|<span data-ttu-id="a8bc9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a8bc9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8bc9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8bc9-122">Authorization</span></span>|<span data-ttu-id="a8bc9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8bc9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8bc9-124">Accept</span></span>|<span data-ttu-id="a8bc9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8bc9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8bc9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8bc9-126">Request body</span></span>
<span data-ttu-id="a8bc9-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="a8bc9-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="a8bc9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8bc9-129">Property</span></span>|<span data-ttu-id="a8bc9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8bc9-130">Type</span></span>|<span data-ttu-id="a8bc9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8bc9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8bc9-132">id</span><span class="sxs-lookup"><span data-stu-id="a8bc9-132">id</span></span>|<span data-ttu-id="a8bc9-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8bc9-133">String</span></span>|<span data-ttu-id="a8bc9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-134">Key of the entity.</span></span> <span data-ttu-id="a8bc9-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a8bc9-136">displayName</span></span>|<span data-ttu-id="a8bc9-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8bc9-137">String</span></span>|<span data-ttu-id="a8bc9-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a8bc9-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-140">descrição</span><span class="sxs-lookup"><span data-stu-id="a8bc9-140">description</span></span>|<span data-ttu-id="a8bc9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8bc9-141">String</span></span>|<span data-ttu-id="a8bc9-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-142">The description of the app.</span></span> <span data-ttu-id="a8bc9-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-144">publicador</span><span class="sxs-lookup"><span data-stu-id="a8bc9-144">publisher</span></span>|<span data-ttu-id="a8bc9-145">String</span><span class="sxs-lookup"><span data-stu-id="a8bc9-145">String</span></span>|<span data-ttu-id="a8bc9-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-146">The publisher of the app.</span></span> <span data-ttu-id="a8bc9-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a8bc9-148">largeIcon</span></span>|[<span data-ttu-id="a8bc9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a8bc9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a8bc9-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a8bc9-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8bc9-152">createdDateTime</span></span>|<span data-ttu-id="a8bc9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8bc9-153">DateTimeOffset</span></span>|<span data-ttu-id="a8bc9-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-154">The date and time the app was created.</span></span> <span data-ttu-id="a8bc9-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8bc9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a8bc9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8bc9-157">DateTimeOffset</span></span>|<span data-ttu-id="a8bc9-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a8bc9-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a8bc9-160">isFeatured</span></span>|<span data-ttu-id="a8bc9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8bc9-161">Boolean</span></span>|<span data-ttu-id="a8bc9-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a8bc9-163">privacyInformationUrl</span></span>|<span data-ttu-id="a8bc9-164">String</span><span class="sxs-lookup"><span data-stu-id="a8bc9-164">String</span></span>|<span data-ttu-id="a8bc9-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-165">The privacy statement Url.</span></span> <span data-ttu-id="a8bc9-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a8bc9-167">informationUrl</span></span>|<span data-ttu-id="a8bc9-168">String</span><span class="sxs-lookup"><span data-stu-id="a8bc9-168">String</span></span>|<span data-ttu-id="a8bc9-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-169">The more information Url.</span></span> <span data-ttu-id="a8bc9-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="a8bc9-171">owner</span></span>|<span data-ttu-id="a8bc9-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8bc9-172">String</span></span>|<span data-ttu-id="a8bc9-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-173">The owner of the app.</span></span> <span data-ttu-id="a8bc9-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-175">developer</span><span class="sxs-lookup"><span data-stu-id="a8bc9-175">developer</span></span>|<span data-ttu-id="a8bc9-176">String</span><span class="sxs-lookup"><span data-stu-id="a8bc9-176">String</span></span>|<span data-ttu-id="a8bc9-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-177">The developer of the app.</span></span> <span data-ttu-id="a8bc9-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-179">notes</span><span class="sxs-lookup"><span data-stu-id="a8bc9-179">notes</span></span>|<span data-ttu-id="a8bc9-180">String</span><span class="sxs-lookup"><span data-stu-id="a8bc9-180">String</span></span>|<span data-ttu-id="a8bc9-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-181">Notes for the app.</span></span> <span data-ttu-id="a8bc9-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8bc9-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="a8bc9-183">publishingState</span></span>|[<span data-ttu-id="a8bc9-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a8bc9-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a8bc9-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-185">The publishing state for the app.</span></span> <span data-ttu-id="a8bc9-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a8bc9-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a8bc9-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a8bc9-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a8bc9-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a8bc9-189">appAvailability</span></span>|[<span data-ttu-id="a8bc9-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="a8bc9-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="a8bc9-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-191">The Application's availability.</span></span> <span data-ttu-id="a8bc9-192">Herdado [de managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a8bc9-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="a8bc9-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a8bc9-194">version</span><span class="sxs-lookup"><span data-stu-id="a8bc9-194">version</span></span>|<span data-ttu-id="a8bc9-195">String</span><span class="sxs-lookup"><span data-stu-id="a8bc9-195">String</span></span>|<span data-ttu-id="a8bc9-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-196">The Application's version.</span></span> <span data-ttu-id="a8bc9-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8bc9-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="a8bc9-198">packageId</span><span class="sxs-lookup"><span data-stu-id="a8bc9-198">packageId</span></span>|<span data-ttu-id="a8bc9-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8bc9-199">String</span></span>|<span data-ttu-id="a8bc9-200">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-200">The app's package ID.</span></span>|
|<span data-ttu-id="a8bc9-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a8bc9-201">appStoreUrl</span></span>|<span data-ttu-id="a8bc9-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8bc9-202">String</span></span>|<span data-ttu-id="a8bc9-203">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-203">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="a8bc9-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a8bc9-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a8bc9-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a8bc9-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="a8bc9-206">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="a8bc9-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8bc9-207">Response</span></span>
<span data-ttu-id="a8bc9-208">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-208">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8bc9-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8bc9-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8bc9-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8bc9-210">Request</span></span>
<span data-ttu-id="a8bc9-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="a8bc9-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8bc9-212">Response</span></span>
<span data-ttu-id="a8bc9-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8bc9-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




