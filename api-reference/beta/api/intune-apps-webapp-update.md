---
title: Atualizar webApp
description: Atualiza as propriedades de um objeto webApp.
author: tfitzmac
ms.openlocfilehash: c64c12aa6e9d29576990ad5f4572250d8cca4023
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346148"
---
# <a name="update-webapp"></a><span data-ttu-id="8c119-103">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="8c119-103">Update webApp</span></span>

> <span data-ttu-id="8c119-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8c119-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c119-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8c119-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c119-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8c119-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c119-107">Atualiza as propriedades de um objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c119-107">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c119-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c119-108">Prerequisites</span></span>
<span data-ttu-id="8c119-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c119-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c119-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c119-111">Permission type</span></span>|<span data-ttu-id="8c119-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c119-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c119-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c119-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c119-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c119-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c119-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c119-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c119-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c119-116">Not supported.</span></span>|
|<span data-ttu-id="8c119-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c119-117">Application</span></span>|<span data-ttu-id="8c119-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c119-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c119-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c119-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8c119-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c119-120">Request headers</span></span>
|<span data-ttu-id="8c119-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c119-121">Header</span></span>|<span data-ttu-id="8c119-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c119-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c119-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c119-123">Authorization</span></span>|<span data-ttu-id="8c119-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c119-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c119-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c119-125">Accept</span></span>|<span data-ttu-id="8c119-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c119-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c119-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c119-127">Request body</span></span>
<span data-ttu-id="8c119-128">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c119-128">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="8c119-129">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c119-129">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="8c119-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c119-130">Property</span></span>|<span data-ttu-id="8c119-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c119-131">Type</span></span>|<span data-ttu-id="8c119-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c119-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c119-133">id</span><span class="sxs-lookup"><span data-stu-id="8c119-133">id</span></span>|<span data-ttu-id="8c119-134">String</span><span class="sxs-lookup"><span data-stu-id="8c119-134">String</span></span>|<span data-ttu-id="8c119-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c119-135">Key of the entity.</span></span> <span data-ttu-id="8c119-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8c119-137">displayName</span></span>|<span data-ttu-id="8c119-138">String</span><span class="sxs-lookup"><span data-stu-id="8c119-138">String</span></span>|<span data-ttu-id="8c119-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8c119-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8c119-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-141">description</span><span class="sxs-lookup"><span data-stu-id="8c119-141">description</span></span>|<span data-ttu-id="8c119-142">String</span><span class="sxs-lookup"><span data-stu-id="8c119-142">String</span></span>|<span data-ttu-id="8c119-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c119-143">The description of the app.</span></span> <span data-ttu-id="8c119-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8c119-145">publisher</span></span>|<span data-ttu-id="8c119-146">String</span><span class="sxs-lookup"><span data-stu-id="8c119-146">String</span></span>|<span data-ttu-id="8c119-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c119-147">The publisher of the app.</span></span> <span data-ttu-id="8c119-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8c119-149">largeIcon</span></span>|[<span data-ttu-id="8c119-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8c119-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8c119-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8c119-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8c119-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c119-153">createdDateTime</span></span>|<span data-ttu-id="8c119-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c119-154">DateTimeOffset</span></span>|<span data-ttu-id="8c119-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c119-155">The date and time the app was created.</span></span> <span data-ttu-id="8c119-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c119-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8c119-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c119-158">DateTimeOffset</span></span>|<span data-ttu-id="8c119-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8c119-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8c119-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8c119-161">isFeatured</span></span>|<span data-ttu-id="8c119-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c119-162">Boolean</span></span>|<span data-ttu-id="8c119-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8c119-164">privacyInformationUrl</span></span>|<span data-ttu-id="8c119-165">String</span><span class="sxs-lookup"><span data-stu-id="8c119-165">String</span></span>|<span data-ttu-id="8c119-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8c119-166">The privacy statement Url.</span></span> <span data-ttu-id="8c119-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8c119-168">informationUrl</span></span>|<span data-ttu-id="8c119-169">String</span><span class="sxs-lookup"><span data-stu-id="8c119-169">String</span></span>|<span data-ttu-id="8c119-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8c119-170">The more information Url.</span></span> <span data-ttu-id="8c119-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-172">owner</span><span class="sxs-lookup"><span data-stu-id="8c119-172">owner</span></span>|<span data-ttu-id="8c119-173">String</span><span class="sxs-lookup"><span data-stu-id="8c119-173">String</span></span>|<span data-ttu-id="8c119-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8c119-174">The owner of the app.</span></span> <span data-ttu-id="8c119-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-176">developer</span><span class="sxs-lookup"><span data-stu-id="8c119-176">developer</span></span>|<span data-ttu-id="8c119-177">String</span><span class="sxs-lookup"><span data-stu-id="8c119-177">String</span></span>|<span data-ttu-id="8c119-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c119-178">The developer of the app.</span></span> <span data-ttu-id="8c119-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-180">Observações</span><span class="sxs-lookup"><span data-stu-id="8c119-180">notes</span></span>|<span data-ttu-id="8c119-181">String</span><span class="sxs-lookup"><span data-stu-id="8c119-181">String</span></span>|<span data-ttu-id="8c119-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c119-182">Notes for the app.</span></span> <span data-ttu-id="8c119-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8c119-184">uploadState</span></span>|<span data-ttu-id="8c119-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8c119-185">Int32</span></span>|<span data-ttu-id="8c119-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="8c119-186">The upload state.</span></span> <span data-ttu-id="8c119-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c119-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c119-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8c119-188">publishingState</span></span>|[<span data-ttu-id="8c119-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8c119-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8c119-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c119-190">The publishing state for the app.</span></span> <span data-ttu-id="8c119-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8c119-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8c119-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c119-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8c119-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8c119-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8c119-194">appUrl</span><span class="sxs-lookup"><span data-stu-id="8c119-194">appUrl</span></span>|<span data-ttu-id="8c119-195">String</span><span class="sxs-lookup"><span data-stu-id="8c119-195">String</span></span>|<span data-ttu-id="8c119-196">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="8c119-196">The web app URL.</span></span>|
|<span data-ttu-id="8c119-197">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="8c119-197">useManagedBrowser</span></span>|<span data-ttu-id="8c119-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c119-198">Boolean</span></span>|<span data-ttu-id="8c119-199">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="8c119-199">Whether or not to use managed browser.</span></span> <span data-ttu-id="8c119-200">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="8c119-200">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="8c119-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c119-201">Response</span></span>
<span data-ttu-id="8c119-202">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune-apps-webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c119-202">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c119-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c119-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c119-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c119-204">Request</span></span>
<span data-ttu-id="8c119-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c119-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 686

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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="8c119-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c119-206">Response</span></span>
<span data-ttu-id="8c119-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c119-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





