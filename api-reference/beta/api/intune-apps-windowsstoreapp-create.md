---
title: Criar windowsStoreApp
description: Criar um novo objeto windowsStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1902c9a26c82f449c3c8c980df995fc3617ad7c9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336282"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="64902-103">Criar windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="64902-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="64902-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64902-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64902-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64902-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64902-106">Criar um novo objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="64902-106">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64902-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64902-107">Prerequisites</span></span>
<span data-ttu-id="64902-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64902-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64902-110">Permission type</span></span>|<span data-ttu-id="64902-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64902-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64902-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64902-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64902-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64902-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64902-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64902-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64902-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64902-115">Not supported.</span></span>|
|<span data-ttu-id="64902-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64902-116">Application</span></span>|<span data-ttu-id="64902-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64902-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64902-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64902-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="64902-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64902-119">Request headers</span></span>
|<span data-ttu-id="64902-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64902-120">Header</span></span>|<span data-ttu-id="64902-121">Valor</span><span class="sxs-lookup"><span data-stu-id="64902-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64902-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64902-122">Authorization</span></span>|<span data-ttu-id="64902-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64902-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64902-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64902-124">Accept</span></span>|<span data-ttu-id="64902-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64902-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64902-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64902-126">Request body</span></span>
<span data-ttu-id="64902-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="64902-127">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="64902-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="64902-128">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="64902-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64902-129">Property</span></span>|<span data-ttu-id="64902-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="64902-130">Type</span></span>|<span data-ttu-id="64902-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="64902-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64902-132">id</span><span class="sxs-lookup"><span data-stu-id="64902-132">id</span></span>|<span data-ttu-id="64902-133">String</span><span class="sxs-lookup"><span data-stu-id="64902-133">String</span></span>|<span data-ttu-id="64902-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="64902-134">Key of the entity.</span></span> <span data-ttu-id="64902-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-136">displayName</span><span class="sxs-lookup"><span data-stu-id="64902-136">displayName</span></span>|<span data-ttu-id="64902-137">String</span><span class="sxs-lookup"><span data-stu-id="64902-137">String</span></span>|<span data-ttu-id="64902-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="64902-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="64902-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-140">descrição</span><span class="sxs-lookup"><span data-stu-id="64902-140">description</span></span>|<span data-ttu-id="64902-141">String</span><span class="sxs-lookup"><span data-stu-id="64902-141">String</span></span>|<span data-ttu-id="64902-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64902-142">The description of the app.</span></span> <span data-ttu-id="64902-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-144">publicador</span><span class="sxs-lookup"><span data-stu-id="64902-144">publisher</span></span>|<span data-ttu-id="64902-145">String</span><span class="sxs-lookup"><span data-stu-id="64902-145">String</span></span>|<span data-ttu-id="64902-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64902-146">The publisher of the app.</span></span> <span data-ttu-id="64902-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="64902-148">largeIcon</span></span>|[<span data-ttu-id="64902-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="64902-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="64902-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="64902-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="64902-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64902-152">createdDateTime</span></span>|<span data-ttu-id="64902-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64902-153">DateTimeOffset</span></span>|<span data-ttu-id="64902-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64902-154">The date and time the app was created.</span></span> <span data-ttu-id="64902-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64902-156">lastModifiedDateTime</span></span>|<span data-ttu-id="64902-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64902-157">DateTimeOffset</span></span>|<span data-ttu-id="64902-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="64902-158">The date and time the app was last modified.</span></span> <span data-ttu-id="64902-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="64902-160">isFeatured</span></span>|<span data-ttu-id="64902-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="64902-161">Boolean</span></span>|<span data-ttu-id="64902-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="64902-163">privacyInformationUrl</span></span>|<span data-ttu-id="64902-164">String</span><span class="sxs-lookup"><span data-stu-id="64902-164">String</span></span>|<span data-ttu-id="64902-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="64902-165">The privacy statement Url.</span></span> <span data-ttu-id="64902-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="64902-167">informationUrl</span></span>|<span data-ttu-id="64902-168">String</span><span class="sxs-lookup"><span data-stu-id="64902-168">String</span></span>|<span data-ttu-id="64902-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="64902-169">The more information Url.</span></span> <span data-ttu-id="64902-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-171">owner</span><span class="sxs-lookup"><span data-stu-id="64902-171">owner</span></span>|<span data-ttu-id="64902-172">String</span><span class="sxs-lookup"><span data-stu-id="64902-172">String</span></span>|<span data-ttu-id="64902-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="64902-173">The owner of the app.</span></span> <span data-ttu-id="64902-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-175">developer</span><span class="sxs-lookup"><span data-stu-id="64902-175">developer</span></span>|<span data-ttu-id="64902-176">String</span><span class="sxs-lookup"><span data-stu-id="64902-176">String</span></span>|<span data-ttu-id="64902-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64902-177">The developer of the app.</span></span> <span data-ttu-id="64902-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-179">notes</span><span class="sxs-lookup"><span data-stu-id="64902-179">notes</span></span>|<span data-ttu-id="64902-180">String</span><span class="sxs-lookup"><span data-stu-id="64902-180">String</span></span>|<span data-ttu-id="64902-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64902-181">Notes for the app.</span></span> <span data-ttu-id="64902-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="64902-183">uploadState</span></span>|<span data-ttu-id="64902-184">Int32</span><span class="sxs-lookup"><span data-stu-id="64902-184">Int32</span></span>|<span data-ttu-id="64902-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="64902-185">The upload state.</span></span> <span data-ttu-id="64902-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="64902-187">publishingState</span></span>|[<span data-ttu-id="64902-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="64902-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="64902-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64902-189">The publishing state for the app.</span></span> <span data-ttu-id="64902-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="64902-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="64902-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64902-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="64902-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="64902-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="64902-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="64902-193">isAssigned</span></span>|<span data-ttu-id="64902-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="64902-194">Boolean</span></span>|<span data-ttu-id="64902-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="64902-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="64902-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64902-197">roleScopeTagIds</span></span>|<span data-ttu-id="64902-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64902-198">String collection</span></span>|<span data-ttu-id="64902-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="64902-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="64902-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="64902-201">dependentAppCount</span></span>|<span data-ttu-id="64902-202">Int32</span><span class="sxs-lookup"><span data-stu-id="64902-202">Int32</span></span>|<span data-ttu-id="64902-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="64902-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="64902-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="64902-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64902-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="64902-205">appStoreUrl</span></span>|<span data-ttu-id="64902-206">String</span><span class="sxs-lookup"><span data-stu-id="64902-206">String</span></span>|<span data-ttu-id="64902-207">A URL da loja de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="64902-207">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="64902-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="64902-208">Response</span></span>
<span data-ttu-id="64902-209">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64902-209">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64902-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64902-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="64902-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64902-211">Request</span></span>
<span data-ttu-id="64902-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64902-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 768

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="64902-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="64902-213">Response</span></span>
<span data-ttu-id="64902-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64902-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 940

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```






