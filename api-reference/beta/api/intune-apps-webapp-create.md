---
title: Criar webApp
description: Cria um novo objeto webApp.
author: tfitzmac
ms.openlocfilehash: 0ebe226b42fb0a35658a08107c9826a7401825db
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330923"
---
# <a name="create-webapp"></a><span data-ttu-id="f7310-103">Criar webApp</span><span class="sxs-lookup"><span data-stu-id="f7310-103">Create webApp</span></span>

> <span data-ttu-id="f7310-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f7310-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7310-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f7310-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7310-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f7310-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7310-107">Cria um novo objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7310-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7310-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7310-108">Prerequisites</span></span>
<span data-ttu-id="f7310-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7310-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7310-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7310-111">Permission type</span></span>|<span data-ttu-id="f7310-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7310-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7310-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7310-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7310-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7310-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7310-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7310-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7310-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7310-116">Not supported.</span></span>|
|<span data-ttu-id="f7310-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7310-117">Application</span></span>|<span data-ttu-id="f7310-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7310-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7310-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7310-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f7310-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7310-120">Request headers</span></span>
|<span data-ttu-id="f7310-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7310-121">Header</span></span>|<span data-ttu-id="f7310-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f7310-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7310-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7310-123">Authorization</span></span>|<span data-ttu-id="f7310-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7310-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7310-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7310-125">Accept</span></span>|<span data-ttu-id="f7310-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7310-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7310-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7310-127">Request body</span></span>
<span data-ttu-id="f7310-128">No corpo da solicitação, forneça uma representação JSON do objeto webApp.</span><span class="sxs-lookup"><span data-stu-id="f7310-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="f7310-129">A tabela a seguir mostra as propriedades obrigatórias ao criar o webApp.</span><span class="sxs-lookup"><span data-stu-id="f7310-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="f7310-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7310-130">Property</span></span>|<span data-ttu-id="f7310-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7310-131">Type</span></span>|<span data-ttu-id="f7310-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7310-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7310-133">id</span><span class="sxs-lookup"><span data-stu-id="f7310-133">id</span></span>|<span data-ttu-id="f7310-134">String</span><span class="sxs-lookup"><span data-stu-id="f7310-134">String</span></span>|<span data-ttu-id="f7310-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7310-135">Key of the entity.</span></span> <span data-ttu-id="f7310-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f7310-137">displayName</span></span>|<span data-ttu-id="f7310-138">String</span><span class="sxs-lookup"><span data-stu-id="f7310-138">String</span></span>|<span data-ttu-id="f7310-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f7310-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f7310-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-141">description</span><span class="sxs-lookup"><span data-stu-id="f7310-141">description</span></span>|<span data-ttu-id="f7310-142">String</span><span class="sxs-lookup"><span data-stu-id="f7310-142">String</span></span>|<span data-ttu-id="f7310-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7310-143">The description of the app.</span></span> <span data-ttu-id="f7310-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f7310-145">publisher</span></span>|<span data-ttu-id="f7310-146">String</span><span class="sxs-lookup"><span data-stu-id="f7310-146">String</span></span>|<span data-ttu-id="f7310-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7310-147">The publisher of the app.</span></span> <span data-ttu-id="f7310-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f7310-149">largeIcon</span></span>|[<span data-ttu-id="f7310-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f7310-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f7310-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f7310-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f7310-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7310-153">createdDateTime</span></span>|<span data-ttu-id="f7310-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7310-154">DateTimeOffset</span></span>|<span data-ttu-id="f7310-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7310-155">The date and time the app was created.</span></span> <span data-ttu-id="f7310-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7310-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f7310-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7310-158">DateTimeOffset</span></span>|<span data-ttu-id="f7310-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f7310-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f7310-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f7310-161">isFeatured</span></span>|<span data-ttu-id="f7310-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7310-162">Boolean</span></span>|<span data-ttu-id="f7310-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f7310-164">privacyInformationUrl</span></span>|<span data-ttu-id="f7310-165">String</span><span class="sxs-lookup"><span data-stu-id="f7310-165">String</span></span>|<span data-ttu-id="f7310-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f7310-166">The privacy statement Url.</span></span> <span data-ttu-id="f7310-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f7310-168">informationUrl</span></span>|<span data-ttu-id="f7310-169">String</span><span class="sxs-lookup"><span data-stu-id="f7310-169">String</span></span>|<span data-ttu-id="f7310-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f7310-170">The more information Url.</span></span> <span data-ttu-id="f7310-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-172">owner</span><span class="sxs-lookup"><span data-stu-id="f7310-172">owner</span></span>|<span data-ttu-id="f7310-173">String</span><span class="sxs-lookup"><span data-stu-id="f7310-173">String</span></span>|<span data-ttu-id="f7310-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f7310-174">The owner of the app.</span></span> <span data-ttu-id="f7310-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-176">developer</span><span class="sxs-lookup"><span data-stu-id="f7310-176">developer</span></span>|<span data-ttu-id="f7310-177">String</span><span class="sxs-lookup"><span data-stu-id="f7310-177">String</span></span>|<span data-ttu-id="f7310-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7310-178">The developer of the app.</span></span> <span data-ttu-id="f7310-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-180">Observações</span><span class="sxs-lookup"><span data-stu-id="f7310-180">notes</span></span>|<span data-ttu-id="f7310-181">String</span><span class="sxs-lookup"><span data-stu-id="f7310-181">String</span></span>|<span data-ttu-id="f7310-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7310-182">Notes for the app.</span></span> <span data-ttu-id="f7310-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f7310-184">uploadState</span></span>|<span data-ttu-id="f7310-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f7310-185">Int32</span></span>|<span data-ttu-id="f7310-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f7310-186">The upload state.</span></span> <span data-ttu-id="f7310-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7310-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7310-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f7310-188">publishingState</span></span>|[<span data-ttu-id="f7310-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f7310-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f7310-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7310-190">The publishing state for the app.</span></span> <span data-ttu-id="f7310-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f7310-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f7310-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7310-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f7310-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f7310-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f7310-194">appUrl</span><span class="sxs-lookup"><span data-stu-id="f7310-194">appUrl</span></span>|<span data-ttu-id="f7310-195">String</span><span class="sxs-lookup"><span data-stu-id="f7310-195">String</span></span>|<span data-ttu-id="f7310-196">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="f7310-196">The web app URL.</span></span>|
|<span data-ttu-id="f7310-197">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="f7310-197">useManagedBrowser</span></span>|<span data-ttu-id="f7310-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7310-198">Boolean</span></span>|<span data-ttu-id="f7310-199">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="f7310-199">Whether or not to use managed browser.</span></span> <span data-ttu-id="f7310-200">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="f7310-200">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="f7310-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7310-201">Response</span></span>
<span data-ttu-id="f7310-202">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7310-202">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7310-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7310-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7310-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7310-204">Request</span></span>
<span data-ttu-id="f7310-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7310-205">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7310-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7310-206">Response</span></span>
<span data-ttu-id="f7310-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7310-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





