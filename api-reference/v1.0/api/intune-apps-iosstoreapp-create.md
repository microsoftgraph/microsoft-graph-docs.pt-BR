---
title: Criar iosStoreApp
description: Cria um novo objeto iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dca2d1092620c10e2f5d8484d3ccdc43903ffd15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002521"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="b03f8-103">Criar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="b03f8-103">Create iosStoreApp</span></span>

> <span data-ttu-id="b03f8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b03f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b03f8-105">Cria um novo objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b03f8-105">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b03f8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b03f8-106">Prerequisites</span></span>
<span data-ttu-id="b03f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b03f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b03f8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b03f8-109">Permission type</span></span>|<span data-ttu-id="b03f8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b03f8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b03f8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b03f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b03f8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b03f8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b03f8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b03f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b03f8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b03f8-114">Not supported.</span></span>|
|<span data-ttu-id="b03f8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b03f8-115">Application</span></span>|<span data-ttu-id="b03f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b03f8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b03f8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b03f8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b03f8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b03f8-118">Request headers</span></span>
|<span data-ttu-id="b03f8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b03f8-119">Header</span></span>|<span data-ttu-id="b03f8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b03f8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b03f8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b03f8-121">Authorization</span></span>|<span data-ttu-id="b03f8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b03f8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b03f8-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b03f8-123">Accept</span></span>|<span data-ttu-id="b03f8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b03f8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b03f8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b03f8-125">Request body</span></span>
<span data-ttu-id="b03f8-126">No corpo da solicitação, forneça uma representação JSON do objeto iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="b03f8-126">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="b03f8-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="b03f8-127">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="b03f8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b03f8-128">Property</span></span>|<span data-ttu-id="b03f8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b03f8-129">Type</span></span>|<span data-ttu-id="b03f8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b03f8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b03f8-131">id</span><span class="sxs-lookup"><span data-stu-id="b03f8-131">id</span></span>|<span data-ttu-id="b03f8-132">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-132">String</span></span>|<span data-ttu-id="b03f8-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b03f8-133">Key of the entity.</span></span> <span data-ttu-id="b03f8-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b03f8-135">displayName</span></span>|<span data-ttu-id="b03f8-136">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-136">String</span></span>|<span data-ttu-id="b03f8-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b03f8-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b03f8-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-139">descrição</span><span class="sxs-lookup"><span data-stu-id="b03f8-139">description</span></span>|<span data-ttu-id="b03f8-140">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-140">String</span></span>|<span data-ttu-id="b03f8-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b03f8-141">The description of the app.</span></span> <span data-ttu-id="b03f8-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-143">publicador</span><span class="sxs-lookup"><span data-stu-id="b03f8-143">publisher</span></span>|<span data-ttu-id="b03f8-144">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-144">String</span></span>|<span data-ttu-id="b03f8-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b03f8-145">The publisher of the app.</span></span> <span data-ttu-id="b03f8-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b03f8-147">largeIcon</span></span>|[<span data-ttu-id="b03f8-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b03f8-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b03f8-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b03f8-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b03f8-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b03f8-151">createdDateTime</span></span>|<span data-ttu-id="b03f8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b03f8-152">DateTimeOffset</span></span>|<span data-ttu-id="b03f8-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b03f8-153">The date and time the app was created.</span></span> <span data-ttu-id="b03f8-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b03f8-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b03f8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b03f8-156">DateTimeOffset</span></span>|<span data-ttu-id="b03f8-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b03f8-157">The date and time the app was last modified.</span></span> <span data-ttu-id="b03f8-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b03f8-159">isFeatured</span></span>|<span data-ttu-id="b03f8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b03f8-160">Boolean</span></span>|<span data-ttu-id="b03f8-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b03f8-162">privacyInformationUrl</span></span>|<span data-ttu-id="b03f8-163">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-163">String</span></span>|<span data-ttu-id="b03f8-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b03f8-164">The privacy statement Url.</span></span> <span data-ttu-id="b03f8-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b03f8-166">informationUrl</span></span>|<span data-ttu-id="b03f8-167">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-167">String</span></span>|<span data-ttu-id="b03f8-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b03f8-168">The more information Url.</span></span> <span data-ttu-id="b03f8-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-170">owner</span><span class="sxs-lookup"><span data-stu-id="b03f8-170">owner</span></span>|<span data-ttu-id="b03f8-171">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-171">String</span></span>|<span data-ttu-id="b03f8-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b03f8-172">The owner of the app.</span></span> <span data-ttu-id="b03f8-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-174">developer</span><span class="sxs-lookup"><span data-stu-id="b03f8-174">developer</span></span>|<span data-ttu-id="b03f8-175">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-175">String</span></span>|<span data-ttu-id="b03f8-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b03f8-176">The developer of the app.</span></span> <span data-ttu-id="b03f8-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-178">notes</span><span class="sxs-lookup"><span data-stu-id="b03f8-178">notes</span></span>|<span data-ttu-id="b03f8-179">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-179">String</span></span>|<span data-ttu-id="b03f8-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b03f8-180">Notes for the app.</span></span> <span data-ttu-id="b03f8-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b03f8-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b03f8-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="b03f8-182">publishingState</span></span>|[<span data-ttu-id="b03f8-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b03f8-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b03f8-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b03f8-184">The publishing state for the app.</span></span> <span data-ttu-id="b03f8-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b03f8-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b03f8-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b03f8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b03f8-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b03f8-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b03f8-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="b03f8-188">bundleId</span></span>|<span data-ttu-id="b03f8-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b03f8-189">String</span></span>|<span data-ttu-id="b03f8-190">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b03f8-190">The Identity Name.</span></span>|
|<span data-ttu-id="b03f8-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b03f8-191">appStoreUrl</span></span>|<span data-ttu-id="b03f8-192">String</span><span class="sxs-lookup"><span data-stu-id="b03f8-192">String</span></span>|<span data-ttu-id="b03f8-193">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="b03f8-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="b03f8-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b03f8-194">applicableDeviceType</span></span>|[<span data-ttu-id="b03f8-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b03f8-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="b03f8-196">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b03f8-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="b03f8-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b03f8-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b03f8-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b03f8-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="b03f8-199">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b03f8-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b03f8-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03f8-200">Response</span></span>
<span data-ttu-id="b03f8-201">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b03f8-201">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b03f8-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b03f8-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="b03f8-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b03f8-203">Request</span></span>
<span data-ttu-id="b03f8-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b03f8-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1006

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
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
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

### <a name="response"></a><span data-ttu-id="b03f8-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03f8-205">Response</span></span>
<span data-ttu-id="b03f8-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b03f8-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1178

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



