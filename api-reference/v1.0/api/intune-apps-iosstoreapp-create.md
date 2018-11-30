---
title: Criar iosStoreApp
description: Cria um novo objeto iosStoreApp.
ms.openlocfilehash: 7dbf1dd5ff0318d054d99bc4f7ae9a8fcfce8523
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005891"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="2a4f4-103">Criar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="2a4f4-103">Create iosStoreApp</span></span>

> <span data-ttu-id="2a4f4-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a4f4-105">Cria um novo objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a4f4-105">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a4f4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a4f4-106">Prerequisites</span></span>
<span data-ttu-id="2a4f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a4f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a4f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a4f4-109">Permission type</span></span>|<span data-ttu-id="2a4f4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a4f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a4f4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4f4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a4f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a4f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-114">Not supported.</span></span>|
|<span data-ttu-id="2a4f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a4f4-115">Application</span></span>|<span data-ttu-id="2a4f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a4f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4f4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2a4f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4f4-118">Request headers</span></span>
|<span data-ttu-id="2a4f4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a4f4-119">Header</span></span>|<span data-ttu-id="2a4f4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2a4f4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a4f4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a4f4-121">Authorization</span></span>|<span data-ttu-id="2a4f4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a4f4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2a4f4-123">Accept</span></span>|<span data-ttu-id="2a4f4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2a4f4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a4f4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4f4-125">Request body</span></span>
<span data-ttu-id="2a4f4-126">No corpo da solicitação, forneça uma representação JSON do objeto iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-126">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="2a4f4-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-127">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="2a4f4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a4f4-128">Property</span></span>|<span data-ttu-id="2a4f4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a4f4-129">Type</span></span>|<span data-ttu-id="2a4f4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4f4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a4f4-131">id</span><span class="sxs-lookup"><span data-stu-id="2a4f4-131">id</span></span>|<span data-ttu-id="2a4f4-132">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-132">String</span></span>|<span data-ttu-id="2a4f4-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-133">Key of the entity.</span></span> <span data-ttu-id="2a4f4-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2a4f4-135">displayName</span></span>|<span data-ttu-id="2a4f4-136">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-136">String</span></span>|<span data-ttu-id="2a4f4-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2a4f4-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-139">description</span><span class="sxs-lookup"><span data-stu-id="2a4f4-139">description</span></span>|<span data-ttu-id="2a4f4-140">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-140">String</span></span>|<span data-ttu-id="2a4f4-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-141">The description of the app.</span></span> <span data-ttu-id="2a4f4-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-143">publisher</span><span class="sxs-lookup"><span data-stu-id="2a4f4-143">publisher</span></span>|<span data-ttu-id="2a4f4-144">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-144">String</span></span>|<span data-ttu-id="2a4f4-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-145">The publisher of the app.</span></span> <span data-ttu-id="2a4f4-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2a4f4-147">largeIcon</span></span>|[<span data-ttu-id="2a4f4-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2a4f4-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2a4f4-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2a4f4-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a4f4-151">createdDateTime</span></span>|<span data-ttu-id="2a4f4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a4f4-152">DateTimeOffset</span></span>|<span data-ttu-id="2a4f4-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-153">The date and time the app was created.</span></span> <span data-ttu-id="2a4f4-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a4f4-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2a4f4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a4f4-156">DateTimeOffset</span></span>|<span data-ttu-id="2a4f4-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-157">The date and time the app was last modified.</span></span> <span data-ttu-id="2a4f4-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2a4f4-159">isFeatured</span></span>|<span data-ttu-id="2a4f4-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="2a4f4-160">Boolean</span></span>|<span data-ttu-id="2a4f4-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2a4f4-162">privacyInformationUrl</span></span>|<span data-ttu-id="2a4f4-163">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-163">String</span></span>|<span data-ttu-id="2a4f4-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-164">The privacy statement Url.</span></span> <span data-ttu-id="2a4f4-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2a4f4-166">informationUrl</span></span>|<span data-ttu-id="2a4f4-167">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-167">String</span></span>|<span data-ttu-id="2a4f4-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-168">The more information Url.</span></span> <span data-ttu-id="2a4f4-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-170">owner</span><span class="sxs-lookup"><span data-stu-id="2a4f4-170">owner</span></span>|<span data-ttu-id="2a4f4-171">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-171">String</span></span>|<span data-ttu-id="2a4f4-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-172">The owner of the app.</span></span> <span data-ttu-id="2a4f4-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-174">developer</span><span class="sxs-lookup"><span data-stu-id="2a4f4-174">developer</span></span>|<span data-ttu-id="2a4f4-175">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-175">String</span></span>|<span data-ttu-id="2a4f4-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-176">The developer of the app.</span></span> <span data-ttu-id="2a4f4-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-178">Observações</span><span class="sxs-lookup"><span data-stu-id="2a4f4-178">notes</span></span>|<span data-ttu-id="2a4f4-179">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-179">String</span></span>|<span data-ttu-id="2a4f4-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-180">Notes for the app.</span></span> <span data-ttu-id="2a4f4-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f4-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a4f4-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="2a4f4-182">publishingState</span></span>|[<span data-ttu-id="2a4f4-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2a4f4-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2a4f4-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-184">The publishing state for the app.</span></span> <span data-ttu-id="2a4f4-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2a4f4-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a4f4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2a4f4-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2a4f4-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="2a4f4-188">bundleId</span></span>|<span data-ttu-id="2a4f4-189">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-189">String</span></span>|<span data-ttu-id="2a4f4-190">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-190">The Identity Name.</span></span>|
|<span data-ttu-id="2a4f4-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2a4f4-191">appStoreUrl</span></span>|<span data-ttu-id="2a4f4-192">String</span><span class="sxs-lookup"><span data-stu-id="2a4f4-192">String</span></span>|<span data-ttu-id="2a4f4-193">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="2a4f4-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="2a4f4-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a4f4-194">applicableDeviceType</span></span>|[<span data-ttu-id="2a4f4-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a4f4-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2a4f4-196">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="2a4f4-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a4f4-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2a4f4-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a4f4-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="2a4f4-199">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="2a4f4-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4f4-200">Response</span></span>
<span data-ttu-id="2a4f4-201">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-201">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a4f4-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a4f4-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a4f4-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4f4-203">Request</span></span>
<span data-ttu-id="2a4f4-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2a4f4-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4f4-205">Response</span></span>
<span data-ttu-id="2a4f4-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a4f4-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



