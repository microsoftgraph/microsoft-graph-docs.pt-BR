---
title: Criar windowsStoreApp
description: Criar um novo objeto windowsStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f180e5c6ace8639100736fcf27c89bb80cf71daa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534978"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="91dca-103">Criar windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="91dca-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="91dca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91dca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91dca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91dca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91dca-106">Criar um novo objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="91dca-106">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91dca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91dca-107">Prerequisites</span></span>
<span data-ttu-id="91dca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91dca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91dca-110">Permission type</span></span>|<span data-ttu-id="91dca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91dca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91dca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91dca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91dca-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91dca-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="91dca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91dca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91dca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91dca-115">Not supported.</span></span>|
|<span data-ttu-id="91dca-116">Application</span><span class="sxs-lookup"><span data-stu-id="91dca-116">Application</span></span>|<span data-ttu-id="91dca-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91dca-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91dca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91dca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="91dca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91dca-119">Request headers</span></span>
|<span data-ttu-id="91dca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91dca-120">Header</span></span>|<span data-ttu-id="91dca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91dca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91dca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91dca-122">Authorization</span></span>|<span data-ttu-id="91dca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91dca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91dca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91dca-124">Accept</span></span>|<span data-ttu-id="91dca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91dca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91dca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91dca-126">Request body</span></span>
<span data-ttu-id="91dca-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="91dca-127">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="91dca-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="91dca-128">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="91dca-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91dca-129">Property</span></span>|<span data-ttu-id="91dca-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="91dca-130">Type</span></span>|<span data-ttu-id="91dca-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="91dca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91dca-132">id</span><span class="sxs-lookup"><span data-stu-id="91dca-132">id</span></span>|<span data-ttu-id="91dca-133">String</span><span class="sxs-lookup"><span data-stu-id="91dca-133">String</span></span>|<span data-ttu-id="91dca-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91dca-134">Key of the entity.</span></span> <span data-ttu-id="91dca-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-136">displayName</span><span class="sxs-lookup"><span data-stu-id="91dca-136">displayName</span></span>|<span data-ttu-id="91dca-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dca-137">String</span></span>|<span data-ttu-id="91dca-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="91dca-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="91dca-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-140">description</span><span class="sxs-lookup"><span data-stu-id="91dca-140">description</span></span>|<span data-ttu-id="91dca-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dca-141">String</span></span>|<span data-ttu-id="91dca-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91dca-142">The description of the app.</span></span> <span data-ttu-id="91dca-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-144">publicador</span><span class="sxs-lookup"><span data-stu-id="91dca-144">publisher</span></span>|<span data-ttu-id="91dca-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dca-145">String</span></span>|<span data-ttu-id="91dca-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91dca-146">The publisher of the app.</span></span> <span data-ttu-id="91dca-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="91dca-148">largeIcon</span></span>|[<span data-ttu-id="91dca-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="91dca-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="91dca-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="91dca-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="91dca-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91dca-152">createdDateTime</span></span>|<span data-ttu-id="91dca-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91dca-153">DateTimeOffset</span></span>|<span data-ttu-id="91dca-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91dca-154">The date and time the app was created.</span></span> <span data-ttu-id="91dca-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91dca-156">lastModifiedDateTime</span></span>|<span data-ttu-id="91dca-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91dca-157">DateTimeOffset</span></span>|<span data-ttu-id="91dca-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="91dca-158">The date and time the app was last modified.</span></span> <span data-ttu-id="91dca-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="91dca-160">isFeatured</span></span>|<span data-ttu-id="91dca-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="91dca-161">Boolean</span></span>|<span data-ttu-id="91dca-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="91dca-163">privacyInformationUrl</span></span>|<span data-ttu-id="91dca-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dca-164">String</span></span>|<span data-ttu-id="91dca-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="91dca-165">The privacy statement Url.</span></span> <span data-ttu-id="91dca-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="91dca-167">informationUrl</span></span>|<span data-ttu-id="91dca-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dca-168">String</span></span>|<span data-ttu-id="91dca-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="91dca-169">The more information Url.</span></span> <span data-ttu-id="91dca-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-171">owner</span><span class="sxs-lookup"><span data-stu-id="91dca-171">owner</span></span>|<span data-ttu-id="91dca-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dca-172">String</span></span>|<span data-ttu-id="91dca-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="91dca-173">The owner of the app.</span></span> <span data-ttu-id="91dca-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-175">developer</span><span class="sxs-lookup"><span data-stu-id="91dca-175">developer</span></span>|<span data-ttu-id="91dca-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91dca-176">String</span></span>|<span data-ttu-id="91dca-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91dca-177">The developer of the app.</span></span> <span data-ttu-id="91dca-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-179">notes</span><span class="sxs-lookup"><span data-stu-id="91dca-179">notes</span></span>|<span data-ttu-id="91dca-180">String</span><span class="sxs-lookup"><span data-stu-id="91dca-180">String</span></span>|<span data-ttu-id="91dca-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91dca-181">Notes for the app.</span></span> <span data-ttu-id="91dca-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="91dca-183">uploadState</span></span>|<span data-ttu-id="91dca-184">Int32</span><span class="sxs-lookup"><span data-stu-id="91dca-184">Int32</span></span>|<span data-ttu-id="91dca-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="91dca-185">The upload state.</span></span> <span data-ttu-id="91dca-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="91dca-187">publishingState</span></span>|[<span data-ttu-id="91dca-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="91dca-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="91dca-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91dca-189">The publishing state for the app.</span></span> <span data-ttu-id="91dca-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="91dca-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="91dca-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="91dca-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="91dca-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="91dca-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="91dca-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="91dca-193">isAssigned</span></span>|<span data-ttu-id="91dca-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="91dca-194">Boolean</span></span>|<span data-ttu-id="91dca-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="91dca-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="91dca-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="91dca-197">roleScopeTagIds</span></span>|<span data-ttu-id="91dca-198">String collection</span><span class="sxs-lookup"><span data-stu-id="91dca-198">String collection</span></span>|<span data-ttu-id="91dca-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="91dca-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="91dca-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="91dca-201">dependentAppCount</span></span>|<span data-ttu-id="91dca-202">Int32</span><span class="sxs-lookup"><span data-stu-id="91dca-202">Int32</span></span>|<span data-ttu-id="91dca-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="91dca-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="91dca-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91dca-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="91dca-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="91dca-205">appStoreUrl</span></span>|<span data-ttu-id="91dca-206">String</span><span class="sxs-lookup"><span data-stu-id="91dca-206">String</span></span>|<span data-ttu-id="91dca-207">A URL da loja de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="91dca-207">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="91dca-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="91dca-208">Response</span></span>
<span data-ttu-id="91dca-209">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91dca-209">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91dca-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91dca-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="91dca-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91dca-211">Request</span></span>
<span data-ttu-id="91dca-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91dca-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91dca-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="91dca-213">Response</span></span>
<span data-ttu-id="91dca-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91dca-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






