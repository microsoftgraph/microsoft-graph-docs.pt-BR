---
title: Atualizar managedIOSStoreApp
description: Atualiza as propriedades de um objeto managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55d57270292fc844669aaf6689429fe3271c45b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453999"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="bd56d-103">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="bd56d-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="bd56d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd56d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd56d-105">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="bd56d-105">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd56d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd56d-106">Prerequisites</span></span>
<span data-ttu-id="bd56d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd56d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd56d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd56d-109">Permission type</span></span>|<span data-ttu-id="bd56d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd56d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd56d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd56d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd56d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd56d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd56d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd56d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd56d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd56d-114">Not supported.</span></span>|
|<span data-ttu-id="bd56d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd56d-115">Application</span></span>|<span data-ttu-id="bd56d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd56d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd56d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd56d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="bd56d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd56d-118">Request headers</span></span>
|<span data-ttu-id="bd56d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd56d-119">Header</span></span>|<span data-ttu-id="bd56d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bd56d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd56d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd56d-121">Authorization</span></span>|<span data-ttu-id="bd56d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd56d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd56d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd56d-123">Accept</span></span>|<span data-ttu-id="bd56d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bd56d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd56d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd56d-125">Request body</span></span>
<span data-ttu-id="bd56d-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="bd56d-126">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="bd56d-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="bd56d-127">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="bd56d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd56d-128">Property</span></span>|<span data-ttu-id="bd56d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd56d-129">Type</span></span>|<span data-ttu-id="bd56d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd56d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd56d-131">id</span><span class="sxs-lookup"><span data-stu-id="bd56d-131">id</span></span>|<span data-ttu-id="bd56d-132">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-132">String</span></span>|<span data-ttu-id="bd56d-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bd56d-133">Key of the entity.</span></span> <span data-ttu-id="bd56d-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bd56d-135">displayName</span></span>|<span data-ttu-id="bd56d-136">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-136">String</span></span>|<span data-ttu-id="bd56d-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bd56d-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bd56d-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-139">description</span><span class="sxs-lookup"><span data-stu-id="bd56d-139">description</span></span>|<span data-ttu-id="bd56d-140">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-140">String</span></span>|<span data-ttu-id="bd56d-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-141">The description of the app.</span></span> <span data-ttu-id="bd56d-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-143">publicador</span><span class="sxs-lookup"><span data-stu-id="bd56d-143">publisher</span></span>|<span data-ttu-id="bd56d-144">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-144">String</span></span>|<span data-ttu-id="bd56d-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-145">The publisher of the app.</span></span> <span data-ttu-id="bd56d-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bd56d-147">largeIcon</span></span>|[<span data-ttu-id="bd56d-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bd56d-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bd56d-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="bd56d-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bd56d-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd56d-151">createdDateTime</span></span>|<span data-ttu-id="bd56d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd56d-152">DateTimeOffset</span></span>|<span data-ttu-id="bd56d-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-153">The date and time the app was created.</span></span> <span data-ttu-id="bd56d-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd56d-155">lastModifiedDateTime</span></span>|<span data-ttu-id="bd56d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd56d-156">DateTimeOffset</span></span>|<span data-ttu-id="bd56d-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bd56d-157">The date and time the app was last modified.</span></span> <span data-ttu-id="bd56d-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bd56d-159">isFeatured</span></span>|<span data-ttu-id="bd56d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd56d-160">Boolean</span></span>|<span data-ttu-id="bd56d-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bd56d-162">privacyInformationUrl</span></span>|<span data-ttu-id="bd56d-163">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-163">String</span></span>|<span data-ttu-id="bd56d-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="bd56d-164">The privacy statement Url.</span></span> <span data-ttu-id="bd56d-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bd56d-166">informationUrl</span></span>|<span data-ttu-id="bd56d-167">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-167">String</span></span>|<span data-ttu-id="bd56d-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bd56d-168">The more information Url.</span></span> <span data-ttu-id="bd56d-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-170">owner</span><span class="sxs-lookup"><span data-stu-id="bd56d-170">owner</span></span>|<span data-ttu-id="bd56d-171">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-171">String</span></span>|<span data-ttu-id="bd56d-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-172">The owner of the app.</span></span> <span data-ttu-id="bd56d-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-174">developer</span><span class="sxs-lookup"><span data-stu-id="bd56d-174">developer</span></span>|<span data-ttu-id="bd56d-175">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-175">String</span></span>|<span data-ttu-id="bd56d-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-176">The developer of the app.</span></span> <span data-ttu-id="bd56d-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-178">notes</span><span class="sxs-lookup"><span data-stu-id="bd56d-178">notes</span></span>|<span data-ttu-id="bd56d-179">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-179">String</span></span>|<span data-ttu-id="bd56d-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-180">Notes for the app.</span></span> <span data-ttu-id="bd56d-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd56d-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="bd56d-182">publishingState</span></span>|[<span data-ttu-id="bd56d-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bd56d-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bd56d-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-184">The publishing state for the app.</span></span> <span data-ttu-id="bd56d-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="bd56d-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bd56d-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bd56d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bd56d-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bd56d-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bd56d-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="bd56d-188">appAvailability</span></span>|[<span data-ttu-id="bd56d-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="bd56d-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="bd56d-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-190">The Application's availability.</span></span> <span data-ttu-id="bd56d-191">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bd56d-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="bd56d-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="bd56d-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="bd56d-193">version</span><span class="sxs-lookup"><span data-stu-id="bd56d-193">version</span></span>|<span data-ttu-id="bd56d-194">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-194">String</span></span>|<span data-ttu-id="bd56d-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd56d-195">The Application's version.</span></span> <span data-ttu-id="bd56d-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd56d-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="bd56d-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="bd56d-197">bundleId</span></span>|<span data-ttu-id="bd56d-198">String</span><span class="sxs-lookup"><span data-stu-id="bd56d-198">String</span></span>|<span data-ttu-id="bd56d-199">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bd56d-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="bd56d-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bd56d-200">appStoreUrl</span></span>|<span data-ttu-id="bd56d-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd56d-201">String</span></span>|<span data-ttu-id="bd56d-202">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="bd56d-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="bd56d-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="bd56d-203">applicableDeviceType</span></span>|[<span data-ttu-id="bd56d-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="bd56d-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="bd56d-205">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="bd56d-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="bd56d-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bd56d-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bd56d-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bd56d-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="bd56d-208">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="bd56d-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="bd56d-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd56d-209">Response</span></span>
<span data-ttu-id="bd56d-210">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd56d-210">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd56d-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd56d-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd56d-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd56d-212">Request</span></span>
<span data-ttu-id="bd56d-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd56d-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="bd56d-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd56d-214">Response</span></span>
<span data-ttu-id="bd56d-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd56d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



