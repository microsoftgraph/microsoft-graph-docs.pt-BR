---
title: Criar webApp
description: Cria um novo objeto webApp.
ms.openlocfilehash: ea048b1beb1c036ea8bc8c1bd4f6e904e446b87c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036586"
---
# <a name="create-webapp"></a><span data-ttu-id="70d41-103">Criar webApp</span><span class="sxs-lookup"><span data-stu-id="70d41-103">Create webApp</span></span>

> <span data-ttu-id="70d41-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="70d41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70d41-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="70d41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70d41-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="70d41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70d41-107">Cria um novo objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="70d41-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70d41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70d41-108">Prerequisites</span></span>
<span data-ttu-id="70d41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70d41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70d41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70d41-111">Permission type</span></span>|<span data-ttu-id="70d41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70d41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70d41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70d41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70d41-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70d41-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70d41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70d41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70d41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70d41-116">Not supported.</span></span>|
|<span data-ttu-id="70d41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70d41-117">Application</span></span>|<span data-ttu-id="70d41-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70d41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70d41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70d41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="70d41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70d41-120">Request headers</span></span>
|<span data-ttu-id="70d41-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70d41-121">Header</span></span>|<span data-ttu-id="70d41-122">Valor</span><span class="sxs-lookup"><span data-stu-id="70d41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70d41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70d41-123">Authorization</span></span>|<span data-ttu-id="70d41-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70d41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70d41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70d41-125">Accept</span></span>|<span data-ttu-id="70d41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70d41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70d41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70d41-127">Request body</span></span>
<span data-ttu-id="70d41-128">No corpo da solicitação, forneça uma representação JSON do objeto webApp.</span><span class="sxs-lookup"><span data-stu-id="70d41-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="70d41-129">A tabela a seguir mostra as propriedades obrigatórias ao criar o webApp.</span><span class="sxs-lookup"><span data-stu-id="70d41-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="70d41-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70d41-130">Property</span></span>|<span data-ttu-id="70d41-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="70d41-131">Type</span></span>|<span data-ttu-id="70d41-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="70d41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70d41-133">id</span><span class="sxs-lookup"><span data-stu-id="70d41-133">id</span></span>|<span data-ttu-id="70d41-134">String</span><span class="sxs-lookup"><span data-stu-id="70d41-134">String</span></span>|<span data-ttu-id="70d41-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="70d41-135">Key of the entity.</span></span> <span data-ttu-id="70d41-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-137">displayName</span><span class="sxs-lookup"><span data-stu-id="70d41-137">displayName</span></span>|<span data-ttu-id="70d41-138">String</span><span class="sxs-lookup"><span data-stu-id="70d41-138">String</span></span>|<span data-ttu-id="70d41-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="70d41-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="70d41-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-141">description</span><span class="sxs-lookup"><span data-stu-id="70d41-141">description</span></span>|<span data-ttu-id="70d41-142">String</span><span class="sxs-lookup"><span data-stu-id="70d41-142">String</span></span>|<span data-ttu-id="70d41-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70d41-143">The description of the app.</span></span> <span data-ttu-id="70d41-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-145">publisher</span><span class="sxs-lookup"><span data-stu-id="70d41-145">publisher</span></span>|<span data-ttu-id="70d41-146">String</span><span class="sxs-lookup"><span data-stu-id="70d41-146">String</span></span>|<span data-ttu-id="70d41-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70d41-147">The publisher of the app.</span></span> <span data-ttu-id="70d41-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="70d41-149">largeIcon</span></span>|[<span data-ttu-id="70d41-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="70d41-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="70d41-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="70d41-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="70d41-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70d41-153">createdDateTime</span></span>|<span data-ttu-id="70d41-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70d41-154">DateTimeOffset</span></span>|<span data-ttu-id="70d41-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70d41-155">The date and time the app was created.</span></span> <span data-ttu-id="70d41-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70d41-157">lastModifiedDateTime</span></span>|<span data-ttu-id="70d41-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70d41-158">DateTimeOffset</span></span>|<span data-ttu-id="70d41-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="70d41-159">The date and time the app was last modified.</span></span> <span data-ttu-id="70d41-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="70d41-161">isFeatured</span></span>|<span data-ttu-id="70d41-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="70d41-162">Boolean</span></span>|<span data-ttu-id="70d41-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="70d41-164">privacyInformationUrl</span></span>|<span data-ttu-id="70d41-165">String</span><span class="sxs-lookup"><span data-stu-id="70d41-165">String</span></span>|<span data-ttu-id="70d41-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="70d41-166">The privacy statement Url.</span></span> <span data-ttu-id="70d41-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="70d41-168">informationUrl</span></span>|<span data-ttu-id="70d41-169">String</span><span class="sxs-lookup"><span data-stu-id="70d41-169">String</span></span>|<span data-ttu-id="70d41-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="70d41-170">The more information Url.</span></span> <span data-ttu-id="70d41-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-172">owner</span><span class="sxs-lookup"><span data-stu-id="70d41-172">owner</span></span>|<span data-ttu-id="70d41-173">String</span><span class="sxs-lookup"><span data-stu-id="70d41-173">String</span></span>|<span data-ttu-id="70d41-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="70d41-174">The owner of the app.</span></span> <span data-ttu-id="70d41-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-176">developer</span><span class="sxs-lookup"><span data-stu-id="70d41-176">developer</span></span>|<span data-ttu-id="70d41-177">String</span><span class="sxs-lookup"><span data-stu-id="70d41-177">String</span></span>|<span data-ttu-id="70d41-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70d41-178">The developer of the app.</span></span> <span data-ttu-id="70d41-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-180">Observações</span><span class="sxs-lookup"><span data-stu-id="70d41-180">notes</span></span>|<span data-ttu-id="70d41-181">String</span><span class="sxs-lookup"><span data-stu-id="70d41-181">String</span></span>|<span data-ttu-id="70d41-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70d41-182">Notes for the app.</span></span> <span data-ttu-id="70d41-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="70d41-184">uploadState</span></span>|<span data-ttu-id="70d41-185">Int32</span><span class="sxs-lookup"><span data-stu-id="70d41-185">Int32</span></span>|<span data-ttu-id="70d41-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="70d41-186">The upload state.</span></span> <span data-ttu-id="70d41-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70d41-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="70d41-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="70d41-188">publishingState</span></span>|[<span data-ttu-id="70d41-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="70d41-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="70d41-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70d41-190">The publishing state for the app.</span></span> <span data-ttu-id="70d41-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="70d41-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="70d41-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="70d41-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="70d41-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="70d41-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="70d41-194">appUrl</span><span class="sxs-lookup"><span data-stu-id="70d41-194">appUrl</span></span>|<span data-ttu-id="70d41-195">String</span><span class="sxs-lookup"><span data-stu-id="70d41-195">String</span></span>|<span data-ttu-id="70d41-196">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="70d41-196">The web app URL.</span></span>|
|<span data-ttu-id="70d41-197">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="70d41-197">useManagedBrowser</span></span>|<span data-ttu-id="70d41-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="70d41-198">Boolean</span></span>|<span data-ttu-id="70d41-199">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="70d41-199">Whether or not to use managed browser.</span></span> <span data-ttu-id="70d41-200">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="70d41-200">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="70d41-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="70d41-201">Response</span></span>
<span data-ttu-id="70d41-202">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70d41-202">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70d41-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70d41-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="70d41-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70d41-204">Request</span></span>
<span data-ttu-id="70d41-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70d41-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 731

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="70d41-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="70d41-206">Response</span></span>
<span data-ttu-id="70d41-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70d41-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 839

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```





