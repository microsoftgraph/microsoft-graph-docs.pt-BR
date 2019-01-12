---
title: Atualizar iosStoreApp
description: Atualiza as propriedades de um objeto iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2939708cc49e056e584f419b16efc8c7d7129ab8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935910"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="19c36-103">Atualizar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="19c36-103">Update iosStoreApp</span></span>

> <span data-ttu-id="19c36-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="19c36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19c36-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="19c36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19c36-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="19c36-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19c36-107">Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="19c36-107">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19c36-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19c36-108">Prerequisites</span></span>
<span data-ttu-id="19c36-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19c36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19c36-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19c36-111">Permission type</span></span>|<span data-ttu-id="19c36-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19c36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19c36-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19c36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19c36-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19c36-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19c36-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19c36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19c36-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19c36-116">Not supported.</span></span>|
|<span data-ttu-id="19c36-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19c36-117">Application</span></span>|<span data-ttu-id="19c36-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19c36-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19c36-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19c36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="19c36-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19c36-120">Request headers</span></span>
|<span data-ttu-id="19c36-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19c36-121">Header</span></span>|<span data-ttu-id="19c36-122">Valor</span><span class="sxs-lookup"><span data-stu-id="19c36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19c36-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19c36-123">Authorization</span></span>|<span data-ttu-id="19c36-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19c36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19c36-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19c36-125">Accept</span></span>|<span data-ttu-id="19c36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19c36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19c36-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19c36-127">Request body</span></span>
<span data-ttu-id="19c36-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="19c36-128">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="19c36-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="19c36-129">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="19c36-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19c36-130">Property</span></span>|<span data-ttu-id="19c36-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="19c36-131">Type</span></span>|<span data-ttu-id="19c36-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="19c36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c36-133">id</span><span class="sxs-lookup"><span data-stu-id="19c36-133">id</span></span>|<span data-ttu-id="19c36-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-134">String</span></span>|<span data-ttu-id="19c36-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="19c36-135">Key of the entity.</span></span> <span data-ttu-id="19c36-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-137">displayName</span><span class="sxs-lookup"><span data-stu-id="19c36-137">displayName</span></span>|<span data-ttu-id="19c36-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-138">String</span></span>|<span data-ttu-id="19c36-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="19c36-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="19c36-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-141">description</span><span class="sxs-lookup"><span data-stu-id="19c36-141">description</span></span>|<span data-ttu-id="19c36-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-142">String</span></span>|<span data-ttu-id="19c36-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19c36-143">The description of the app.</span></span> <span data-ttu-id="19c36-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-145">publisher</span><span class="sxs-lookup"><span data-stu-id="19c36-145">publisher</span></span>|<span data-ttu-id="19c36-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-146">String</span></span>|<span data-ttu-id="19c36-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19c36-147">The publisher of the app.</span></span> <span data-ttu-id="19c36-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="19c36-149">largeIcon</span></span>|[<span data-ttu-id="19c36-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="19c36-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="19c36-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="19c36-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="19c36-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19c36-153">createdDateTime</span></span>|<span data-ttu-id="19c36-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19c36-154">DateTimeOffset</span></span>|<span data-ttu-id="19c36-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19c36-155">The date and time the app was created.</span></span> <span data-ttu-id="19c36-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19c36-157">lastModifiedDateTime</span></span>|<span data-ttu-id="19c36-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19c36-158">DateTimeOffset</span></span>|<span data-ttu-id="19c36-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="19c36-159">The date and time the app was last modified.</span></span> <span data-ttu-id="19c36-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="19c36-161">isFeatured</span></span>|<span data-ttu-id="19c36-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="19c36-162">Boolean</span></span>|<span data-ttu-id="19c36-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="19c36-164">privacyInformationUrl</span></span>|<span data-ttu-id="19c36-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-165">String</span></span>|<span data-ttu-id="19c36-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="19c36-166">The privacy statement Url.</span></span> <span data-ttu-id="19c36-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="19c36-168">informationUrl</span></span>|<span data-ttu-id="19c36-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-169">String</span></span>|<span data-ttu-id="19c36-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="19c36-170">The more information Url.</span></span> <span data-ttu-id="19c36-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-172">owner</span><span class="sxs-lookup"><span data-stu-id="19c36-172">owner</span></span>|<span data-ttu-id="19c36-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-173">String</span></span>|<span data-ttu-id="19c36-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="19c36-174">The owner of the app.</span></span> <span data-ttu-id="19c36-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-176">developer</span><span class="sxs-lookup"><span data-stu-id="19c36-176">developer</span></span>|<span data-ttu-id="19c36-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-177">String</span></span>|<span data-ttu-id="19c36-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19c36-178">The developer of the app.</span></span> <span data-ttu-id="19c36-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-180">Observações</span><span class="sxs-lookup"><span data-stu-id="19c36-180">notes</span></span>|<span data-ttu-id="19c36-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-181">String</span></span>|<span data-ttu-id="19c36-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19c36-182">Notes for the app.</span></span> <span data-ttu-id="19c36-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="19c36-184">uploadState</span></span>|<span data-ttu-id="19c36-185">Int32</span><span class="sxs-lookup"><span data-stu-id="19c36-185">Int32</span></span>|<span data-ttu-id="19c36-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="19c36-186">The upload state.</span></span> <span data-ttu-id="19c36-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="19c36-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="19c36-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="19c36-188">publishingState</span></span>|[<span data-ttu-id="19c36-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="19c36-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="19c36-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19c36-190">The publishing state for the app.</span></span> <span data-ttu-id="19c36-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="19c36-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="19c36-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="19c36-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="19c36-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="19c36-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="19c36-194">bundleId</span><span class="sxs-lookup"><span data-stu-id="19c36-194">bundleId</span></span>|<span data-ttu-id="19c36-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-195">String</span></span>|<span data-ttu-id="19c36-196">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="19c36-196">The Identity Name.</span></span>|
|<span data-ttu-id="19c36-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="19c36-197">appStoreUrl</span></span>|<span data-ttu-id="19c36-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19c36-198">String</span></span>|<span data-ttu-id="19c36-199">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="19c36-199">The Apple App Store URL</span></span>|
|<span data-ttu-id="19c36-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="19c36-200">applicableDeviceType</span></span>|[<span data-ttu-id="19c36-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="19c36-201">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="19c36-202">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="19c36-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="19c36-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="19c36-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="19c36-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="19c36-204">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="19c36-205">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="19c36-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="19c36-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="19c36-206">Response</span></span>
<span data-ttu-id="19c36-207">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19c36-207">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19c36-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19c36-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="19c36-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19c36-209">Request</span></span>
<span data-ttu-id="19c36-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19c36-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1042

{
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

### <a name="response"></a><span data-ttu-id="19c36-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="19c36-211">Response</span></span>
<span data-ttu-id="19c36-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19c36-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1200

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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





