---
title: Criar windowsPhone81StoreApp
description: Crie um novo objeto de windowsPhone81StoreApp.
ms.openlocfilehash: d937eb98ca1eec2d9b6f8fc562f926bc43c3b356
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039589"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="c2610-103">Criar windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="c2610-103">Create windowsPhone81StoreApp</span></span>

> <span data-ttu-id="c2610-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c2610-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2610-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c2610-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2610-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c2610-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2610-107">Crie um novo objeto de [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c2610-107">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2610-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2610-108">Prerequisites</span></span>
<span data-ttu-id="c2610-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2610-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2610-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2610-111">Permission type</span></span>|<span data-ttu-id="c2610-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c2610-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2610-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2610-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2610-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2610-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2610-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2610-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2610-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2610-116">Not supported.</span></span>|
|<span data-ttu-id="c2610-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2610-117">Application</span></span>|<span data-ttu-id="c2610-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2610-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2610-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2610-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c2610-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2610-120">Request headers</span></span>
|<span data-ttu-id="c2610-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2610-121">Header</span></span>|<span data-ttu-id="c2610-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c2610-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2610-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2610-123">Authorization</span></span>|<span data-ttu-id="c2610-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2610-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2610-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2610-125">Accept</span></span>|<span data-ttu-id="c2610-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2610-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2610-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2610-127">Request body</span></span>
<span data-ttu-id="c2610-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="c2610-128">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="c2610-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="c2610-129">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="c2610-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2610-130">Property</span></span>|<span data-ttu-id="c2610-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2610-131">Type</span></span>|<span data-ttu-id="c2610-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2610-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2610-133">id</span><span class="sxs-lookup"><span data-stu-id="c2610-133">id</span></span>|<span data-ttu-id="c2610-134">String</span><span class="sxs-lookup"><span data-stu-id="c2610-134">String</span></span>|<span data-ttu-id="c2610-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c2610-135">Key of the entity.</span></span> <span data-ttu-id="c2610-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c2610-137">displayName</span></span>|<span data-ttu-id="c2610-138">String</span><span class="sxs-lookup"><span data-stu-id="c2610-138">String</span></span>|<span data-ttu-id="c2610-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c2610-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c2610-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-141">description</span><span class="sxs-lookup"><span data-stu-id="c2610-141">description</span></span>|<span data-ttu-id="c2610-142">String</span><span class="sxs-lookup"><span data-stu-id="c2610-142">String</span></span>|<span data-ttu-id="c2610-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c2610-143">The description of the app.</span></span> <span data-ttu-id="c2610-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c2610-145">publisher</span></span>|<span data-ttu-id="c2610-146">String</span><span class="sxs-lookup"><span data-stu-id="c2610-146">String</span></span>|<span data-ttu-id="c2610-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c2610-147">The publisher of the app.</span></span> <span data-ttu-id="c2610-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c2610-149">largeIcon</span></span>|[<span data-ttu-id="c2610-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c2610-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c2610-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="c2610-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c2610-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2610-153">createdDateTime</span></span>|<span data-ttu-id="c2610-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2610-154">DateTimeOffset</span></span>|<span data-ttu-id="c2610-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c2610-155">The date and time the app was created.</span></span> <span data-ttu-id="c2610-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2610-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c2610-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2610-158">DateTimeOffset</span></span>|<span data-ttu-id="c2610-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c2610-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c2610-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c2610-161">isFeatured</span></span>|<span data-ttu-id="c2610-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="c2610-162">Boolean</span></span>|<span data-ttu-id="c2610-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c2610-164">privacyInformationUrl</span></span>|<span data-ttu-id="c2610-165">String</span><span class="sxs-lookup"><span data-stu-id="c2610-165">String</span></span>|<span data-ttu-id="c2610-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c2610-166">The privacy statement Url.</span></span> <span data-ttu-id="c2610-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c2610-168">informationUrl</span></span>|<span data-ttu-id="c2610-169">String</span><span class="sxs-lookup"><span data-stu-id="c2610-169">String</span></span>|<span data-ttu-id="c2610-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c2610-170">The more information Url.</span></span> <span data-ttu-id="c2610-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-172">owner</span><span class="sxs-lookup"><span data-stu-id="c2610-172">owner</span></span>|<span data-ttu-id="c2610-173">String</span><span class="sxs-lookup"><span data-stu-id="c2610-173">String</span></span>|<span data-ttu-id="c2610-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c2610-174">The owner of the app.</span></span> <span data-ttu-id="c2610-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-176">developer</span><span class="sxs-lookup"><span data-stu-id="c2610-176">developer</span></span>|<span data-ttu-id="c2610-177">String</span><span class="sxs-lookup"><span data-stu-id="c2610-177">String</span></span>|<span data-ttu-id="c2610-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c2610-178">The developer of the app.</span></span> <span data-ttu-id="c2610-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-180">Observações</span><span class="sxs-lookup"><span data-stu-id="c2610-180">notes</span></span>|<span data-ttu-id="c2610-181">String</span><span class="sxs-lookup"><span data-stu-id="c2610-181">String</span></span>|<span data-ttu-id="c2610-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c2610-182">Notes for the app.</span></span> <span data-ttu-id="c2610-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c2610-184">uploadState</span></span>|<span data-ttu-id="c2610-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c2610-185">Int32</span></span>|<span data-ttu-id="c2610-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="c2610-186">The upload state.</span></span> <span data-ttu-id="c2610-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2610-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2610-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c2610-188">publishingState</span></span>|[<span data-ttu-id="c2610-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c2610-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c2610-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c2610-190">The publishing state for the app.</span></span> <span data-ttu-id="c2610-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="c2610-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c2610-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2610-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c2610-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c2610-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c2610-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c2610-194">appStoreUrl</span></span>|<span data-ttu-id="c2610-195">String</span><span class="sxs-lookup"><span data-stu-id="c2610-195">String</span></span>|<span data-ttu-id="c2610-196">A URL do repositório do Windows Phone 8.1 app.</span><span class="sxs-lookup"><span data-stu-id="c2610-196">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="c2610-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2610-197">Response</span></span>
<span data-ttu-id="c2610-198">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2610-198">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2610-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2610-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2610-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2610-200">Request</span></span>
<span data-ttu-id="c2610-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2610-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 727

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="c2610-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2610-202">Response</span></span>
<span data-ttu-id="c2610-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2610-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 835

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





