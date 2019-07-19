---
title: Atualizar windowsPhone81StoreApp
description: Atualiza as propriedades de um objeto windowsPhone81StoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdbe426057edc1487e616aa5af2513642b1c3e94
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972904"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="e6934-103">Atualizar windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="e6934-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="e6934-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6934-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6934-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6934-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6934-106">Atualiza as propriedades de um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e6934-106">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6934-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6934-107">Prerequisites</span></span>
<span data-ttu-id="e6934-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6934-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6934-110">Permission type</span></span>|<span data-ttu-id="e6934-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6934-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6934-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6934-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6934-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6934-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6934-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6934-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6934-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6934-115">Not supported.</span></span>|
|<span data-ttu-id="e6934-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6934-116">Application</span></span>|<span data-ttu-id="e6934-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6934-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6934-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6934-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e6934-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6934-119">Request headers</span></span>
|<span data-ttu-id="e6934-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6934-120">Header</span></span>|<span data-ttu-id="e6934-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e6934-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6934-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6934-122">Authorization</span></span>|<span data-ttu-id="e6934-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6934-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6934-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6934-124">Accept</span></span>|<span data-ttu-id="e6934-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6934-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6934-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6934-126">Request body</span></span>
<span data-ttu-id="e6934-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e6934-127">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="e6934-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span><span class="sxs-lookup"><span data-stu-id="e6934-128">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="e6934-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6934-129">Property</span></span>|<span data-ttu-id="e6934-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6934-130">Type</span></span>|<span data-ttu-id="e6934-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6934-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6934-132">id</span><span class="sxs-lookup"><span data-stu-id="e6934-132">id</span></span>|<span data-ttu-id="e6934-133">String</span><span class="sxs-lookup"><span data-stu-id="e6934-133">String</span></span>|<span data-ttu-id="e6934-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e6934-134">Key of the entity.</span></span> <span data-ttu-id="e6934-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e6934-136">displayName</span></span>|<span data-ttu-id="e6934-137">String</span><span class="sxs-lookup"><span data-stu-id="e6934-137">String</span></span>|<span data-ttu-id="e6934-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e6934-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e6934-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-140">descrição</span><span class="sxs-lookup"><span data-stu-id="e6934-140">description</span></span>|<span data-ttu-id="e6934-141">String</span><span class="sxs-lookup"><span data-stu-id="e6934-141">String</span></span>|<span data-ttu-id="e6934-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6934-142">The description of the app.</span></span> <span data-ttu-id="e6934-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-144">publicador</span><span class="sxs-lookup"><span data-stu-id="e6934-144">publisher</span></span>|<span data-ttu-id="e6934-145">String</span><span class="sxs-lookup"><span data-stu-id="e6934-145">String</span></span>|<span data-ttu-id="e6934-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6934-146">The publisher of the app.</span></span> <span data-ttu-id="e6934-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e6934-148">largeIcon</span></span>|[<span data-ttu-id="e6934-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e6934-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e6934-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e6934-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e6934-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6934-152">createdDateTime</span></span>|<span data-ttu-id="e6934-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6934-153">DateTimeOffset</span></span>|<span data-ttu-id="e6934-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6934-154">The date and time the app was created.</span></span> <span data-ttu-id="e6934-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6934-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e6934-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6934-157">DateTimeOffset</span></span>|<span data-ttu-id="e6934-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e6934-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e6934-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e6934-160">isFeatured</span></span>|<span data-ttu-id="e6934-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6934-161">Boolean</span></span>|<span data-ttu-id="e6934-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e6934-163">privacyInformationUrl</span></span>|<span data-ttu-id="e6934-164">String</span><span class="sxs-lookup"><span data-stu-id="e6934-164">String</span></span>|<span data-ttu-id="e6934-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e6934-165">The privacy statement Url.</span></span> <span data-ttu-id="e6934-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e6934-167">informationUrl</span></span>|<span data-ttu-id="e6934-168">String</span><span class="sxs-lookup"><span data-stu-id="e6934-168">String</span></span>|<span data-ttu-id="e6934-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e6934-169">The more information Url.</span></span> <span data-ttu-id="e6934-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-171">owner</span><span class="sxs-lookup"><span data-stu-id="e6934-171">owner</span></span>|<span data-ttu-id="e6934-172">String</span><span class="sxs-lookup"><span data-stu-id="e6934-172">String</span></span>|<span data-ttu-id="e6934-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e6934-173">The owner of the app.</span></span> <span data-ttu-id="e6934-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-175">developer</span><span class="sxs-lookup"><span data-stu-id="e6934-175">developer</span></span>|<span data-ttu-id="e6934-176">String</span><span class="sxs-lookup"><span data-stu-id="e6934-176">String</span></span>|<span data-ttu-id="e6934-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6934-177">The developer of the app.</span></span> <span data-ttu-id="e6934-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-179">notes</span><span class="sxs-lookup"><span data-stu-id="e6934-179">notes</span></span>|<span data-ttu-id="e6934-180">String</span><span class="sxs-lookup"><span data-stu-id="e6934-180">String</span></span>|<span data-ttu-id="e6934-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6934-181">Notes for the app.</span></span> <span data-ttu-id="e6934-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e6934-183">uploadState</span></span>|<span data-ttu-id="e6934-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e6934-184">Int32</span></span>|<span data-ttu-id="e6934-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e6934-185">The upload state.</span></span> <span data-ttu-id="e6934-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e6934-187">publishingState</span></span>|[<span data-ttu-id="e6934-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e6934-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e6934-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6934-189">The publishing state for the app.</span></span> <span data-ttu-id="e6934-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e6934-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e6934-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e6934-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e6934-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e6934-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e6934-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e6934-193">isAssigned</span></span>|<span data-ttu-id="e6934-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6934-194">Boolean</span></span>|<span data-ttu-id="e6934-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e6934-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e6934-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6934-197">roleScopeTagIds</span></span>|<span data-ttu-id="e6934-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6934-198">String collection</span></span>|<span data-ttu-id="e6934-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e6934-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e6934-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e6934-201">dependentAppCount</span></span>|<span data-ttu-id="e6934-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e6934-202">Int32</span></span>|<span data-ttu-id="e6934-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e6934-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e6934-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6934-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6934-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e6934-205">appStoreUrl</span></span>|<span data-ttu-id="e6934-206">String</span><span class="sxs-lookup"><span data-stu-id="e6934-206">String</span></span>|<span data-ttu-id="e6934-207">A URL da loja de aplicativos do Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="e6934-207">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="e6934-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6934-208">Response</span></span>
<span data-ttu-id="e6934-209">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6934-209">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6934-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6934-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6934-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6934-211">Request</span></span>
<span data-ttu-id="e6934-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6934-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="e6934-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6934-213">Response</span></span>
<span data-ttu-id="e6934-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6934-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





