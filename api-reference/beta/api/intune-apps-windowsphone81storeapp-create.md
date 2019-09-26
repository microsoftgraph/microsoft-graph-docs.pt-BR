---
title: Criar windowsPhone81StoreApp
description: Criar um novo objeto windowsPhone81StoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 055c58faaede2ec482c85c832b966aeadeaf195b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171859"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="d7c10-103">Criar windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="d7c10-103">Create windowsPhone81StoreApp</span></span>

> <span data-ttu-id="d7c10-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7c10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7c10-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7c10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7c10-106">Criar um novo objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d7c10-106">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7c10-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7c10-107">Prerequisites</span></span>
<span data-ttu-id="d7c10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7c10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7c10-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7c10-110">Permission type</span></span>|<span data-ttu-id="d7c10-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7c10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7c10-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7c10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7c10-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c10-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7c10-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7c10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7c10-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7c10-115">Not supported.</span></span>|
|<span data-ttu-id="d7c10-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7c10-116">Application</span></span>|<span data-ttu-id="d7c10-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c10-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7c10-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7c10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d7c10-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c10-119">Request headers</span></span>
|<span data-ttu-id="d7c10-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7c10-120">Header</span></span>|<span data-ttu-id="d7c10-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d7c10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7c10-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7c10-122">Authorization</span></span>|<span data-ttu-id="d7c10-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7c10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7c10-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7c10-124">Accept</span></span>|<span data-ttu-id="d7c10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7c10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7c10-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c10-126">Request body</span></span>
<span data-ttu-id="d7c10-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="d7c10-127">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="d7c10-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="d7c10-128">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="d7c10-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7c10-129">Property</span></span>|<span data-ttu-id="d7c10-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7c10-130">Type</span></span>|<span data-ttu-id="d7c10-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7c10-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7c10-132">id</span><span class="sxs-lookup"><span data-stu-id="d7c10-132">id</span></span>|<span data-ttu-id="d7c10-133">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-133">String</span></span>|<span data-ttu-id="d7c10-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d7c10-134">Key of the entity.</span></span> <span data-ttu-id="d7c10-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d7c10-136">displayName</span></span>|<span data-ttu-id="d7c10-137">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-137">String</span></span>|<span data-ttu-id="d7c10-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d7c10-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d7c10-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-140">descrição</span><span class="sxs-lookup"><span data-stu-id="d7c10-140">description</span></span>|<span data-ttu-id="d7c10-141">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-141">String</span></span>|<span data-ttu-id="d7c10-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d7c10-142">The description of the app.</span></span> <span data-ttu-id="d7c10-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-144">publicador</span><span class="sxs-lookup"><span data-stu-id="d7c10-144">publisher</span></span>|<span data-ttu-id="d7c10-145">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-145">String</span></span>|<span data-ttu-id="d7c10-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d7c10-146">The publisher of the app.</span></span> <span data-ttu-id="d7c10-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d7c10-148">largeIcon</span></span>|[<span data-ttu-id="d7c10-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d7c10-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d7c10-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d7c10-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d7c10-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7c10-152">createdDateTime</span></span>|<span data-ttu-id="d7c10-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7c10-153">DateTimeOffset</span></span>|<span data-ttu-id="d7c10-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d7c10-154">The date and time the app was created.</span></span> <span data-ttu-id="d7c10-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7c10-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d7c10-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7c10-157">DateTimeOffset</span></span>|<span data-ttu-id="d7c10-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d7c10-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d7c10-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d7c10-160">isFeatured</span></span>|<span data-ttu-id="d7c10-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7c10-161">Boolean</span></span>|<span data-ttu-id="d7c10-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d7c10-163">privacyInformationUrl</span></span>|<span data-ttu-id="d7c10-164">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-164">String</span></span>|<span data-ttu-id="d7c10-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d7c10-165">The privacy statement Url.</span></span> <span data-ttu-id="d7c10-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d7c10-167">informationUrl</span></span>|<span data-ttu-id="d7c10-168">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-168">String</span></span>|<span data-ttu-id="d7c10-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d7c10-169">The more information Url.</span></span> <span data-ttu-id="d7c10-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-171">owner</span><span class="sxs-lookup"><span data-stu-id="d7c10-171">owner</span></span>|<span data-ttu-id="d7c10-172">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-172">String</span></span>|<span data-ttu-id="d7c10-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d7c10-173">The owner of the app.</span></span> <span data-ttu-id="d7c10-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-175">developer</span><span class="sxs-lookup"><span data-stu-id="d7c10-175">developer</span></span>|<span data-ttu-id="d7c10-176">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-176">String</span></span>|<span data-ttu-id="d7c10-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d7c10-177">The developer of the app.</span></span> <span data-ttu-id="d7c10-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-179">notes</span><span class="sxs-lookup"><span data-stu-id="d7c10-179">notes</span></span>|<span data-ttu-id="d7c10-180">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-180">String</span></span>|<span data-ttu-id="d7c10-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d7c10-181">Notes for the app.</span></span> <span data-ttu-id="d7c10-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d7c10-183">uploadState</span></span>|<span data-ttu-id="d7c10-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c10-184">Int32</span></span>|<span data-ttu-id="d7c10-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="d7c10-185">The upload state.</span></span> <span data-ttu-id="d7c10-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d7c10-187">publishingState</span></span>|[<span data-ttu-id="d7c10-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d7c10-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d7c10-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d7c10-189">The publishing state for the app.</span></span> <span data-ttu-id="d7c10-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d7c10-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d7c10-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7c10-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d7c10-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d7c10-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d7c10-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d7c10-193">isAssigned</span></span>|<span data-ttu-id="d7c10-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7c10-194">Boolean</span></span>|<span data-ttu-id="d7c10-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="d7c10-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d7c10-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7c10-197">roleScopeTagIds</span></span>|<span data-ttu-id="d7c10-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7c10-198">String collection</span></span>|<span data-ttu-id="d7c10-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d7c10-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d7c10-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d7c10-201">dependentAppCount</span></span>|<span data-ttu-id="d7c10-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c10-202">Int32</span></span>|<span data-ttu-id="d7c10-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="d7c10-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d7c10-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7c10-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7c10-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d7c10-205">appStoreUrl</span></span>|<span data-ttu-id="d7c10-206">String</span><span class="sxs-lookup"><span data-stu-id="d7c10-206">String</span></span>|<span data-ttu-id="d7c10-207">A URL da loja de aplicativos do Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="d7c10-207">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="d7c10-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c10-208">Response</span></span>
<span data-ttu-id="d7c10-209">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7c10-209">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7c10-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7c10-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7c10-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c10-211">Request</span></span>
<span data-ttu-id="d7c10-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7c10-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 775

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

### <a name="response"></a><span data-ttu-id="d7c10-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c10-213">Response</span></span>
<span data-ttu-id="d7c10-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7c10-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 947

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




