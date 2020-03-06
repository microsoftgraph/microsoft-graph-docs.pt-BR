---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 666b3f38d626180a2be1b2bb64088a5b50fb111b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516163"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="47c28-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="47c28-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="47c28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47c28-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47c28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47c28-106">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c28-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47c28-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47c28-107">Prerequisites</span></span>
<span data-ttu-id="47c28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="47c28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="47c28-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47c28-110">Permission type</span></span>|<span data-ttu-id="47c28-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47c28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47c28-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47c28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47c28-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c28-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47c28-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47c28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47c28-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47c28-115">Not supported.</span></span>|
|<span data-ttu-id="47c28-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47c28-116">Application</span></span>|<span data-ttu-id="47c28-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c28-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47c28-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47c28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="47c28-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47c28-119">Request headers</span></span>
|<span data-ttu-id="47c28-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47c28-120">Header</span></span>|<span data-ttu-id="47c28-121">Valor</span><span class="sxs-lookup"><span data-stu-id="47c28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47c28-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="47c28-122">Authorization</span></span>|<span data-ttu-id="47c28-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47c28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47c28-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47c28-124">Accept</span></span>|<span data-ttu-id="47c28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47c28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47c28-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47c28-126">Request body</span></span>
<span data-ttu-id="47c28-127">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="47c28-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="47c28-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="47c28-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="47c28-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47c28-129">Property</span></span>|<span data-ttu-id="47c28-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="47c28-130">Type</span></span>|<span data-ttu-id="47c28-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="47c28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47c28-132">id</span><span class="sxs-lookup"><span data-stu-id="47c28-132">id</span></span>|<span data-ttu-id="47c28-133">String</span><span class="sxs-lookup"><span data-stu-id="47c28-133">String</span></span>|<span data-ttu-id="47c28-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47c28-134">Key of the entity.</span></span> <span data-ttu-id="47c28-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-136">displayName</span><span class="sxs-lookup"><span data-stu-id="47c28-136">displayName</span></span>|<span data-ttu-id="47c28-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47c28-137">String</span></span>|<span data-ttu-id="47c28-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="47c28-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="47c28-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-140">description</span><span class="sxs-lookup"><span data-stu-id="47c28-140">description</span></span>|<span data-ttu-id="47c28-141">String</span><span class="sxs-lookup"><span data-stu-id="47c28-141">String</span></span>|<span data-ttu-id="47c28-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47c28-142">The description of the app.</span></span> <span data-ttu-id="47c28-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-144">publicador</span><span class="sxs-lookup"><span data-stu-id="47c28-144">publisher</span></span>|<span data-ttu-id="47c28-145">String</span><span class="sxs-lookup"><span data-stu-id="47c28-145">String</span></span>|<span data-ttu-id="47c28-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47c28-146">The publisher of the app.</span></span> <span data-ttu-id="47c28-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="47c28-148">largeIcon</span></span>|[<span data-ttu-id="47c28-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="47c28-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="47c28-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="47c28-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="47c28-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47c28-152">createdDateTime</span></span>|<span data-ttu-id="47c28-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c28-153">DateTimeOffset</span></span>|<span data-ttu-id="47c28-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47c28-154">The date and time the app was created.</span></span> <span data-ttu-id="47c28-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47c28-156">lastModifiedDateTime</span></span>|<span data-ttu-id="47c28-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c28-157">DateTimeOffset</span></span>|<span data-ttu-id="47c28-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="47c28-158">The date and time the app was last modified.</span></span> <span data-ttu-id="47c28-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="47c28-160">isFeatured</span></span>|<span data-ttu-id="47c28-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="47c28-161">Boolean</span></span>|<span data-ttu-id="47c28-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="47c28-163">privacyInformationUrl</span></span>|<span data-ttu-id="47c28-164">String</span><span class="sxs-lookup"><span data-stu-id="47c28-164">String</span></span>|<span data-ttu-id="47c28-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="47c28-165">The privacy statement Url.</span></span> <span data-ttu-id="47c28-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="47c28-167">informationUrl</span></span>|<span data-ttu-id="47c28-168">String</span><span class="sxs-lookup"><span data-stu-id="47c28-168">String</span></span>|<span data-ttu-id="47c28-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="47c28-169">The more information Url.</span></span> <span data-ttu-id="47c28-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-171">owner</span><span class="sxs-lookup"><span data-stu-id="47c28-171">owner</span></span>|<span data-ttu-id="47c28-172">String</span><span class="sxs-lookup"><span data-stu-id="47c28-172">String</span></span>|<span data-ttu-id="47c28-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="47c28-173">The owner of the app.</span></span> <span data-ttu-id="47c28-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-175">developer</span><span class="sxs-lookup"><span data-stu-id="47c28-175">developer</span></span>|<span data-ttu-id="47c28-176">String</span><span class="sxs-lookup"><span data-stu-id="47c28-176">String</span></span>|<span data-ttu-id="47c28-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47c28-177">The developer of the app.</span></span> <span data-ttu-id="47c28-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-179">notes</span><span class="sxs-lookup"><span data-stu-id="47c28-179">notes</span></span>|<span data-ttu-id="47c28-180">String</span><span class="sxs-lookup"><span data-stu-id="47c28-180">String</span></span>|<span data-ttu-id="47c28-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47c28-181">Notes for the app.</span></span> <span data-ttu-id="47c28-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="47c28-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="47c28-183">publishingState</span></span>|[<span data-ttu-id="47c28-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="47c28-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="47c28-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47c28-185">The publishing state for the app.</span></span> <span data-ttu-id="47c28-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="47c28-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="47c28-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c28-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="47c28-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="47c28-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="47c28-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="47c28-189">appAvailability</span></span>|[<span data-ttu-id="47c28-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="47c28-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="47c28-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47c28-191">The Application's availability.</span></span> <span data-ttu-id="47c28-192">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c28-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="47c28-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="47c28-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="47c28-194">version</span><span class="sxs-lookup"><span data-stu-id="47c28-194">version</span></span>|<span data-ttu-id="47c28-195">String</span><span class="sxs-lookup"><span data-stu-id="47c28-195">String</span></span>|<span data-ttu-id="47c28-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="47c28-196">The Application's version.</span></span> <span data-ttu-id="47c28-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="47c28-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="47c28-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="47c28-198">bundleId</span></span>|<span data-ttu-id="47c28-199">String</span><span class="sxs-lookup"><span data-stu-id="47c28-199">String</span></span>|<span data-ttu-id="47c28-200">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="47c28-200">The app's Bundle ID.</span></span>|
|<span data-ttu-id="47c28-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="47c28-201">appStoreUrl</span></span>|<span data-ttu-id="47c28-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47c28-202">String</span></span>|<span data-ttu-id="47c28-203">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="47c28-203">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="47c28-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="47c28-204">applicableDeviceType</span></span>|[<span data-ttu-id="47c28-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="47c28-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="47c28-206">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="47c28-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="47c28-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="47c28-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="47c28-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="47c28-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="47c28-209">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="47c28-209">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="47c28-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c28-210">Response</span></span>
<span data-ttu-id="47c28-211">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47c28-211">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47c28-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47c28-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="47c28-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47c28-213">Request</span></span>
<span data-ttu-id="47c28-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47c28-214">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47c28-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c28-215">Response</span></span>
<span data-ttu-id="47c28-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47c28-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




