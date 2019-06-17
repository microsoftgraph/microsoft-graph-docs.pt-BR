---
title: Atualizar windowsStoreApp
description: Atualiza as propriedades de um objeto windowsStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9bf99d5c84fcf942fd978d105e1b6e95bc608ff
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972750"
---
# <a name="update-windowsstoreapp"></a><span data-ttu-id="97637-103">Atualizar windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="97637-103">Update windowsStoreApp</span></span>

> <span data-ttu-id="97637-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97637-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97637-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97637-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97637-106">Atualiza as propriedades de um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="97637-106">Update the properties of a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97637-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97637-107">Prerequisites</span></span>
<span data-ttu-id="97637-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97637-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97637-110">Permission type</span></span>|<span data-ttu-id="97637-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97637-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97637-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97637-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97637-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97637-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="97637-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97637-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97637-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97637-115">Not supported.</span></span>|
|<span data-ttu-id="97637-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97637-116">Application</span></span>|<span data-ttu-id="97637-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97637-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97637-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97637-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="97637-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97637-119">Request headers</span></span>
|<span data-ttu-id="97637-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97637-120">Header</span></span>|<span data-ttu-id="97637-121">Valor</span><span class="sxs-lookup"><span data-stu-id="97637-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97637-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="97637-122">Authorization</span></span>|<span data-ttu-id="97637-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97637-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97637-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97637-124">Accept</span></span>|<span data-ttu-id="97637-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97637-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97637-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97637-126">Request body</span></span>
<span data-ttu-id="97637-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="97637-127">In the request body, supply a JSON representation for the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

<span data-ttu-id="97637-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="97637-128">The following table shows the properties that are required when you create the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

|<span data-ttu-id="97637-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97637-129">Property</span></span>|<span data-ttu-id="97637-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="97637-130">Type</span></span>|<span data-ttu-id="97637-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="97637-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97637-132">id</span><span class="sxs-lookup"><span data-stu-id="97637-132">id</span></span>|<span data-ttu-id="97637-133">String</span><span class="sxs-lookup"><span data-stu-id="97637-133">String</span></span>|<span data-ttu-id="97637-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="97637-134">Key of the entity.</span></span> <span data-ttu-id="97637-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-136">displayName</span><span class="sxs-lookup"><span data-stu-id="97637-136">displayName</span></span>|<span data-ttu-id="97637-137">String</span><span class="sxs-lookup"><span data-stu-id="97637-137">String</span></span>|<span data-ttu-id="97637-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="97637-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="97637-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-140">descrição</span><span class="sxs-lookup"><span data-stu-id="97637-140">description</span></span>|<span data-ttu-id="97637-141">String</span><span class="sxs-lookup"><span data-stu-id="97637-141">String</span></span>|<span data-ttu-id="97637-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97637-142">The description of the app.</span></span> <span data-ttu-id="97637-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-144">publicador</span><span class="sxs-lookup"><span data-stu-id="97637-144">publisher</span></span>|<span data-ttu-id="97637-145">String</span><span class="sxs-lookup"><span data-stu-id="97637-145">String</span></span>|<span data-ttu-id="97637-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97637-146">The publisher of the app.</span></span> <span data-ttu-id="97637-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="97637-148">largeIcon</span></span>|[<span data-ttu-id="97637-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="97637-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="97637-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="97637-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="97637-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97637-152">createdDateTime</span></span>|<span data-ttu-id="97637-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97637-153">DateTimeOffset</span></span>|<span data-ttu-id="97637-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97637-154">The date and time the app was created.</span></span> <span data-ttu-id="97637-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97637-156">lastModifiedDateTime</span></span>|<span data-ttu-id="97637-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97637-157">DateTimeOffset</span></span>|<span data-ttu-id="97637-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="97637-158">The date and time the app was last modified.</span></span> <span data-ttu-id="97637-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="97637-160">isFeatured</span></span>|<span data-ttu-id="97637-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="97637-161">Boolean</span></span>|<span data-ttu-id="97637-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="97637-163">privacyInformationUrl</span></span>|<span data-ttu-id="97637-164">String</span><span class="sxs-lookup"><span data-stu-id="97637-164">String</span></span>|<span data-ttu-id="97637-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="97637-165">The privacy statement Url.</span></span> <span data-ttu-id="97637-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="97637-167">informationUrl</span></span>|<span data-ttu-id="97637-168">String</span><span class="sxs-lookup"><span data-stu-id="97637-168">String</span></span>|<span data-ttu-id="97637-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="97637-169">The more information Url.</span></span> <span data-ttu-id="97637-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-171">owner</span><span class="sxs-lookup"><span data-stu-id="97637-171">owner</span></span>|<span data-ttu-id="97637-172">String</span><span class="sxs-lookup"><span data-stu-id="97637-172">String</span></span>|<span data-ttu-id="97637-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="97637-173">The owner of the app.</span></span> <span data-ttu-id="97637-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-175">developer</span><span class="sxs-lookup"><span data-stu-id="97637-175">developer</span></span>|<span data-ttu-id="97637-176">String</span><span class="sxs-lookup"><span data-stu-id="97637-176">String</span></span>|<span data-ttu-id="97637-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97637-177">The developer of the app.</span></span> <span data-ttu-id="97637-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-179">notes</span><span class="sxs-lookup"><span data-stu-id="97637-179">notes</span></span>|<span data-ttu-id="97637-180">String</span><span class="sxs-lookup"><span data-stu-id="97637-180">String</span></span>|<span data-ttu-id="97637-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97637-181">Notes for the app.</span></span> <span data-ttu-id="97637-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="97637-183">uploadState</span></span>|<span data-ttu-id="97637-184">Int32</span><span class="sxs-lookup"><span data-stu-id="97637-184">Int32</span></span>|<span data-ttu-id="97637-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="97637-185">The upload state.</span></span> <span data-ttu-id="97637-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="97637-187">publishingState</span></span>|[<span data-ttu-id="97637-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="97637-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="97637-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97637-189">The publishing state for the app.</span></span> <span data-ttu-id="97637-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="97637-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="97637-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="97637-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="97637-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="97637-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="97637-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="97637-193">isAssigned</span></span>|<span data-ttu-id="97637-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="97637-194">Boolean</span></span>|<span data-ttu-id="97637-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="97637-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="97637-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97637-197">roleScopeTagIds</span></span>|<span data-ttu-id="97637-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="97637-198">String collection</span></span>|<span data-ttu-id="97637-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="97637-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="97637-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="97637-201">dependentAppCount</span></span>|<span data-ttu-id="97637-202">Int32</span><span class="sxs-lookup"><span data-stu-id="97637-202">Int32</span></span>|<span data-ttu-id="97637-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="97637-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="97637-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97637-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97637-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="97637-205">appStoreUrl</span></span>|<span data-ttu-id="97637-206">String</span><span class="sxs-lookup"><span data-stu-id="97637-206">String</span></span>|<span data-ttu-id="97637-207">A URL da loja de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="97637-207">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="97637-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="97637-208">Response</span></span>
<span data-ttu-id="97637-209">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97637-209">If successful, this method returns a `200 OK` response code and an updated [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97637-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97637-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="97637-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97637-211">Request</span></span>
<span data-ttu-id="97637-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97637-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="97637-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="97637-213">Response</span></span>
<span data-ttu-id="97637-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97637-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





