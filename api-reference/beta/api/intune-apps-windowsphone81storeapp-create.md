---
title: Criar windowsPhone81StoreApp
description: Criar um novo objeto windowsPhone81StoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a230127739381d7510985665b4a453be29cdd3a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393496"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="5c906-103">Criar windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="5c906-103">Create windowsPhone81StoreApp</span></span>

<span data-ttu-id="5c906-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c906-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c906-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c906-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c906-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c906-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c906-107">Criar um novo objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="5c906-107">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c906-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c906-108">Prerequisites</span></span>
<span data-ttu-id="5c906-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c906-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c906-111">Permission type</span></span>|<span data-ttu-id="5c906-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c906-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c906-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c906-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c906-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c906-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c906-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c906-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c906-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c906-116">Not supported.</span></span>|
|<span data-ttu-id="5c906-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c906-117">Application</span></span>|<span data-ttu-id="5c906-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c906-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c906-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c906-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5c906-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c906-120">Request headers</span></span>
|<span data-ttu-id="5c906-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c906-121">Header</span></span>|<span data-ttu-id="5c906-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5c906-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c906-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c906-123">Authorization</span></span>|<span data-ttu-id="5c906-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c906-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c906-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c906-125">Accept</span></span>|<span data-ttu-id="5c906-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c906-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c906-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c906-127">Request body</span></span>
<span data-ttu-id="5c906-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="5c906-128">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="5c906-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="5c906-129">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="5c906-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c906-130">Property</span></span>|<span data-ttu-id="5c906-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c906-131">Type</span></span>|<span data-ttu-id="5c906-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c906-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c906-133">id</span><span class="sxs-lookup"><span data-stu-id="5c906-133">id</span></span>|<span data-ttu-id="5c906-134">String</span><span class="sxs-lookup"><span data-stu-id="5c906-134">String</span></span>|<span data-ttu-id="5c906-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5c906-135">Key of the entity.</span></span> <span data-ttu-id="5c906-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5c906-137">displayName</span></span>|<span data-ttu-id="5c906-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c906-138">String</span></span>|<span data-ttu-id="5c906-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="5c906-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5c906-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-141">description</span><span class="sxs-lookup"><span data-stu-id="5c906-141">description</span></span>|<span data-ttu-id="5c906-142">String</span><span class="sxs-lookup"><span data-stu-id="5c906-142">String</span></span>|<span data-ttu-id="5c906-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c906-143">The description of the app.</span></span> <span data-ttu-id="5c906-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-145">publicador</span><span class="sxs-lookup"><span data-stu-id="5c906-145">publisher</span></span>|<span data-ttu-id="5c906-146">String</span><span class="sxs-lookup"><span data-stu-id="5c906-146">String</span></span>|<span data-ttu-id="5c906-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c906-147">The publisher of the app.</span></span> <span data-ttu-id="5c906-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5c906-149">largeIcon</span></span>|[<span data-ttu-id="5c906-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5c906-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5c906-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="5c906-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5c906-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c906-153">createdDateTime</span></span>|<span data-ttu-id="5c906-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c906-154">DateTimeOffset</span></span>|<span data-ttu-id="5c906-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c906-155">The date and time the app was created.</span></span> <span data-ttu-id="5c906-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c906-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5c906-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c906-158">DateTimeOffset</span></span>|<span data-ttu-id="5c906-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5c906-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5c906-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5c906-161">isFeatured</span></span>|<span data-ttu-id="5c906-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c906-162">Boolean</span></span>|<span data-ttu-id="5c906-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5c906-164">privacyInformationUrl</span></span>|<span data-ttu-id="5c906-165">String</span><span class="sxs-lookup"><span data-stu-id="5c906-165">String</span></span>|<span data-ttu-id="5c906-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5c906-166">The privacy statement Url.</span></span> <span data-ttu-id="5c906-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5c906-168">informationUrl</span></span>|<span data-ttu-id="5c906-169">String</span><span class="sxs-lookup"><span data-stu-id="5c906-169">String</span></span>|<span data-ttu-id="5c906-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5c906-170">The more information Url.</span></span> <span data-ttu-id="5c906-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-172">owner</span><span class="sxs-lookup"><span data-stu-id="5c906-172">owner</span></span>|<span data-ttu-id="5c906-173">String</span><span class="sxs-lookup"><span data-stu-id="5c906-173">String</span></span>|<span data-ttu-id="5c906-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5c906-174">The owner of the app.</span></span> <span data-ttu-id="5c906-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-176">developer</span><span class="sxs-lookup"><span data-stu-id="5c906-176">developer</span></span>|<span data-ttu-id="5c906-177">String</span><span class="sxs-lookup"><span data-stu-id="5c906-177">String</span></span>|<span data-ttu-id="5c906-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c906-178">The developer of the app.</span></span> <span data-ttu-id="5c906-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-180">notes</span><span class="sxs-lookup"><span data-stu-id="5c906-180">notes</span></span>|<span data-ttu-id="5c906-181">String</span><span class="sxs-lookup"><span data-stu-id="5c906-181">String</span></span>|<span data-ttu-id="5c906-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c906-182">Notes for the app.</span></span> <span data-ttu-id="5c906-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5c906-184">uploadState</span></span>|<span data-ttu-id="5c906-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5c906-185">Int32</span></span>|<span data-ttu-id="5c906-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="5c906-186">The upload state.</span></span> <span data-ttu-id="5c906-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="5c906-188">publishingState</span></span>|[<span data-ttu-id="5c906-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5c906-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5c906-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c906-190">The publishing state for the app.</span></span> <span data-ttu-id="5c906-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="5c906-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5c906-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c906-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="5c906-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5c906-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5c906-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5c906-194">isAssigned</span></span>|<span data-ttu-id="5c906-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c906-195">Boolean</span></span>|<span data-ttu-id="5c906-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="5c906-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5c906-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c906-198">roleScopeTagIds</span></span>|<span data-ttu-id="5c906-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5c906-199">String collection</span></span>|<span data-ttu-id="5c906-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="5c906-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5c906-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="5c906-202">dependentAppCount</span></span>|<span data-ttu-id="5c906-203">Int32</span><span class="sxs-lookup"><span data-stu-id="5c906-203">Int32</span></span>|<span data-ttu-id="5c906-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="5c906-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5c906-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c906-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5c906-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5c906-206">appStoreUrl</span></span>|<span data-ttu-id="5c906-207">String</span><span class="sxs-lookup"><span data-stu-id="5c906-207">String</span></span>|<span data-ttu-id="5c906-208">A URL da loja de aplicativos do Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="5c906-208">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="5c906-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c906-209">Response</span></span>
<span data-ttu-id="5c906-210">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c906-210">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c906-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c906-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c906-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c906-212">Request</span></span>
<span data-ttu-id="5c906-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c906-213">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c906-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c906-214">Response</span></span>
<span data-ttu-id="5c906-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c906-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



