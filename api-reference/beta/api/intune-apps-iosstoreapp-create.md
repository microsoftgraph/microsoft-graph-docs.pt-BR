---
title: Criar iosStoreApp
description: Cria um novo objeto iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a600146fac5e1f9af704bd9acfb65cb622fea08a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825248"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="92402-103">Criar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="92402-103">Create iosStoreApp</span></span>

> <span data-ttu-id="92402-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92402-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92402-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92402-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92402-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="92402-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92402-107">Cria um novo objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="92402-107">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92402-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92402-108">Prerequisites</span></span>
<span data-ttu-id="92402-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92402-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92402-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92402-111">Permission type</span></span>|<span data-ttu-id="92402-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92402-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92402-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92402-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92402-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92402-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92402-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92402-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92402-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92402-116">Not supported.</span></span>|
|<span data-ttu-id="92402-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92402-117">Application</span></span>|<span data-ttu-id="92402-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92402-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92402-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92402-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="92402-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92402-120">Request headers</span></span>
|<span data-ttu-id="92402-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92402-121">Header</span></span>|<span data-ttu-id="92402-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92402-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92402-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92402-123">Authorization</span></span>|<span data-ttu-id="92402-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92402-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92402-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92402-125">Accept</span></span>|<span data-ttu-id="92402-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92402-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92402-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92402-127">Request body</span></span>
<span data-ttu-id="92402-128">No corpo da solicitação, forneça uma representação JSON do objeto iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="92402-128">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="92402-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="92402-129">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="92402-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92402-130">Property</span></span>|<span data-ttu-id="92402-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92402-131">Type</span></span>|<span data-ttu-id="92402-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92402-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92402-133">id</span><span class="sxs-lookup"><span data-stu-id="92402-133">id</span></span>|<span data-ttu-id="92402-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-134">String</span></span>|<span data-ttu-id="92402-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92402-135">Key of the entity.</span></span> <span data-ttu-id="92402-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-137">displayName</span><span class="sxs-lookup"><span data-stu-id="92402-137">displayName</span></span>|<span data-ttu-id="92402-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-138">String</span></span>|<span data-ttu-id="92402-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="92402-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="92402-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-141">description</span><span class="sxs-lookup"><span data-stu-id="92402-141">description</span></span>|<span data-ttu-id="92402-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-142">String</span></span>|<span data-ttu-id="92402-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92402-143">The description of the app.</span></span> <span data-ttu-id="92402-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-145">publisher</span><span class="sxs-lookup"><span data-stu-id="92402-145">publisher</span></span>|<span data-ttu-id="92402-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-146">String</span></span>|<span data-ttu-id="92402-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92402-147">The publisher of the app.</span></span> <span data-ttu-id="92402-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="92402-149">largeIcon</span></span>|[<span data-ttu-id="92402-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="92402-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="92402-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="92402-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="92402-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92402-153">createdDateTime</span></span>|<span data-ttu-id="92402-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92402-154">DateTimeOffset</span></span>|<span data-ttu-id="92402-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92402-155">The date and time the app was created.</span></span> <span data-ttu-id="92402-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92402-157">lastModifiedDateTime</span></span>|<span data-ttu-id="92402-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92402-158">DateTimeOffset</span></span>|<span data-ttu-id="92402-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="92402-159">The date and time the app was last modified.</span></span> <span data-ttu-id="92402-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="92402-161">isFeatured</span></span>|<span data-ttu-id="92402-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="92402-162">Boolean</span></span>|<span data-ttu-id="92402-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="92402-164">privacyInformationUrl</span></span>|<span data-ttu-id="92402-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-165">String</span></span>|<span data-ttu-id="92402-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="92402-166">The privacy statement Url.</span></span> <span data-ttu-id="92402-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="92402-168">informationUrl</span></span>|<span data-ttu-id="92402-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-169">String</span></span>|<span data-ttu-id="92402-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="92402-170">The more information Url.</span></span> <span data-ttu-id="92402-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-172">owner</span><span class="sxs-lookup"><span data-stu-id="92402-172">owner</span></span>|<span data-ttu-id="92402-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-173">String</span></span>|<span data-ttu-id="92402-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="92402-174">The owner of the app.</span></span> <span data-ttu-id="92402-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-176">developer</span><span class="sxs-lookup"><span data-stu-id="92402-176">developer</span></span>|<span data-ttu-id="92402-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-177">String</span></span>|<span data-ttu-id="92402-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92402-178">The developer of the app.</span></span> <span data-ttu-id="92402-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-180">Observações</span><span class="sxs-lookup"><span data-stu-id="92402-180">notes</span></span>|<span data-ttu-id="92402-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-181">String</span></span>|<span data-ttu-id="92402-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92402-182">Notes for the app.</span></span> <span data-ttu-id="92402-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="92402-184">uploadState</span></span>|<span data-ttu-id="92402-185">Int32</span><span class="sxs-lookup"><span data-stu-id="92402-185">Int32</span></span>|<span data-ttu-id="92402-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="92402-186">The upload state.</span></span> <span data-ttu-id="92402-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="92402-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="92402-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="92402-188">publishingState</span></span>|[<span data-ttu-id="92402-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="92402-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="92402-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92402-190">The publishing state for the app.</span></span> <span data-ttu-id="92402-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="92402-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="92402-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92402-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="92402-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="92402-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="92402-194">bundleId</span><span class="sxs-lookup"><span data-stu-id="92402-194">bundleId</span></span>|<span data-ttu-id="92402-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-195">String</span></span>|<span data-ttu-id="92402-196">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="92402-196">The Identity Name.</span></span>|
|<span data-ttu-id="92402-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="92402-197">appStoreUrl</span></span>|<span data-ttu-id="92402-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92402-198">String</span></span>|<span data-ttu-id="92402-199">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="92402-199">The Apple App Store URL</span></span>|
|<span data-ttu-id="92402-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="92402-200">applicableDeviceType</span></span>|[<span data-ttu-id="92402-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="92402-201">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="92402-202">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="92402-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="92402-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="92402-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="92402-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="92402-204">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="92402-205">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="92402-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="92402-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="92402-206">Response</span></span>
<span data-ttu-id="92402-207">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92402-207">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92402-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92402-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="92402-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92402-209">Request</span></span>
<span data-ttu-id="92402-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92402-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1092

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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

### <a name="response"></a><span data-ttu-id="92402-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="92402-211">Response</span></span>
<span data-ttu-id="92402-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92402-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





