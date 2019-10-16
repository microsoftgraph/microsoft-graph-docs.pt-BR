---
title: Atualizar windowsPhone81StoreApp
description: Atualiza as propriedades de um objeto windowsPhone81StoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa16f27a377f1577bcb173749f60e3f85ef213f2
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534999"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="d3422-103">Atualizar windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="d3422-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="d3422-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3422-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3422-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3422-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3422-106">Atualiza as propriedades de um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d3422-106">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3422-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3422-107">Prerequisites</span></span>
<span data-ttu-id="d3422-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3422-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3422-110">Permission type</span></span>|<span data-ttu-id="d3422-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3422-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3422-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3422-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3422-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3422-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d3422-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3422-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3422-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3422-115">Not supported.</span></span>|
|<span data-ttu-id="d3422-116">Application</span><span class="sxs-lookup"><span data-stu-id="d3422-116">Application</span></span>|<span data-ttu-id="d3422-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3422-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3422-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3422-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d3422-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3422-119">Request headers</span></span>
|<span data-ttu-id="d3422-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3422-120">Header</span></span>|<span data-ttu-id="d3422-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d3422-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3422-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3422-122">Authorization</span></span>|<span data-ttu-id="d3422-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3422-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3422-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3422-124">Accept</span></span>|<span data-ttu-id="d3422-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3422-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3422-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3422-126">Request body</span></span>
<span data-ttu-id="d3422-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d3422-127">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="d3422-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3422-128">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="d3422-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3422-129">Property</span></span>|<span data-ttu-id="d3422-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3422-130">Type</span></span>|<span data-ttu-id="d3422-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3422-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3422-132">id</span><span class="sxs-lookup"><span data-stu-id="d3422-132">id</span></span>|<span data-ttu-id="d3422-133">String</span><span class="sxs-lookup"><span data-stu-id="d3422-133">String</span></span>|<span data-ttu-id="d3422-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d3422-134">Key of the entity.</span></span> <span data-ttu-id="d3422-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d3422-136">displayName</span></span>|<span data-ttu-id="d3422-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3422-137">String</span></span>|<span data-ttu-id="d3422-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d3422-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d3422-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-140">description</span><span class="sxs-lookup"><span data-stu-id="d3422-140">description</span></span>|<span data-ttu-id="d3422-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3422-141">String</span></span>|<span data-ttu-id="d3422-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3422-142">The description of the app.</span></span> <span data-ttu-id="d3422-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-144">publicador</span><span class="sxs-lookup"><span data-stu-id="d3422-144">publisher</span></span>|<span data-ttu-id="d3422-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3422-145">String</span></span>|<span data-ttu-id="d3422-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3422-146">The publisher of the app.</span></span> <span data-ttu-id="d3422-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d3422-148">largeIcon</span></span>|[<span data-ttu-id="d3422-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d3422-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d3422-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d3422-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d3422-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3422-152">createdDateTime</span></span>|<span data-ttu-id="d3422-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3422-153">DateTimeOffset</span></span>|<span data-ttu-id="d3422-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3422-154">The date and time the app was created.</span></span> <span data-ttu-id="d3422-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3422-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d3422-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3422-157">DateTimeOffset</span></span>|<span data-ttu-id="d3422-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d3422-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d3422-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d3422-160">isFeatured</span></span>|<span data-ttu-id="d3422-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3422-161">Boolean</span></span>|<span data-ttu-id="d3422-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d3422-163">privacyInformationUrl</span></span>|<span data-ttu-id="d3422-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3422-164">String</span></span>|<span data-ttu-id="d3422-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d3422-165">The privacy statement Url.</span></span> <span data-ttu-id="d3422-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d3422-167">informationUrl</span></span>|<span data-ttu-id="d3422-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3422-168">String</span></span>|<span data-ttu-id="d3422-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d3422-169">The more information Url.</span></span> <span data-ttu-id="d3422-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-171">owner</span><span class="sxs-lookup"><span data-stu-id="d3422-171">owner</span></span>|<span data-ttu-id="d3422-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3422-172">String</span></span>|<span data-ttu-id="d3422-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d3422-173">The owner of the app.</span></span> <span data-ttu-id="d3422-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-175">developer</span><span class="sxs-lookup"><span data-stu-id="d3422-175">developer</span></span>|<span data-ttu-id="d3422-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3422-176">String</span></span>|<span data-ttu-id="d3422-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3422-177">The developer of the app.</span></span> <span data-ttu-id="d3422-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-179">notes</span><span class="sxs-lookup"><span data-stu-id="d3422-179">notes</span></span>|<span data-ttu-id="d3422-180">String</span><span class="sxs-lookup"><span data-stu-id="d3422-180">String</span></span>|<span data-ttu-id="d3422-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3422-181">Notes for the app.</span></span> <span data-ttu-id="d3422-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d3422-183">uploadState</span></span>|<span data-ttu-id="d3422-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d3422-184">Int32</span></span>|<span data-ttu-id="d3422-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="d3422-185">The upload state.</span></span> <span data-ttu-id="d3422-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d3422-187">publishingState</span></span>|[<span data-ttu-id="d3422-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d3422-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d3422-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3422-189">The publishing state for the app.</span></span> <span data-ttu-id="d3422-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d3422-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d3422-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3422-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d3422-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d3422-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d3422-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d3422-193">isAssigned</span></span>|<span data-ttu-id="d3422-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3422-194">Boolean</span></span>|<span data-ttu-id="d3422-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="d3422-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d3422-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d3422-197">roleScopeTagIds</span></span>|<span data-ttu-id="d3422-198">String collection</span><span class="sxs-lookup"><span data-stu-id="d3422-198">String collection</span></span>|<span data-ttu-id="d3422-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d3422-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d3422-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d3422-201">dependentAppCount</span></span>|<span data-ttu-id="d3422-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d3422-202">Int32</span></span>|<span data-ttu-id="d3422-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="d3422-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d3422-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3422-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3422-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d3422-205">appStoreUrl</span></span>|<span data-ttu-id="d3422-206">String</span><span class="sxs-lookup"><span data-stu-id="d3422-206">String</span></span>|<span data-ttu-id="d3422-207">A URL da loja de aplicativos do Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="d3422-207">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="d3422-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3422-208">Response</span></span>
<span data-ttu-id="d3422-209">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3422-209">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3422-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3422-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3422-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3422-211">Request</span></span>
<span data-ttu-id="d3422-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3422-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3422-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3422-213">Response</span></span>
<span data-ttu-id="d3422-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3422-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






