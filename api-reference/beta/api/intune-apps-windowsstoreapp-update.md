---
title: Atualizar windowsStoreApp
description: Atualiza as propriedades de um objeto windowsStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55f24b23f1b028e18fd91f09ddb363f490c49910
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780494"
---
# <a name="update-windowsstoreapp"></a><span data-ttu-id="b3515-103">Atualizar windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="b3515-103">Update windowsStoreApp</span></span>

> <span data-ttu-id="b3515-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3515-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3515-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3515-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3515-106">Atualiza as propriedades de um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b3515-106">Update the properties of a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3515-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3515-107">Prerequisites</span></span>
<span data-ttu-id="b3515-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3515-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3515-110">Permission type</span></span>|<span data-ttu-id="b3515-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3515-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3515-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3515-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3515-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3515-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3515-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3515-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3515-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3515-115">Not supported.</span></span>|
|<span data-ttu-id="b3515-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3515-116">Application</span></span>|<span data-ttu-id="b3515-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3515-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3515-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3515-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b3515-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3515-119">Request headers</span></span>
|<span data-ttu-id="b3515-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3515-120">Header</span></span>|<span data-ttu-id="b3515-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b3515-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3515-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3515-122">Authorization</span></span>|<span data-ttu-id="b3515-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3515-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3515-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3515-124">Accept</span></span>|<span data-ttu-id="b3515-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3515-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3515-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3515-126">Request body</span></span>
<span data-ttu-id="b3515-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b3515-127">In the request body, supply a JSON representation for the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

<span data-ttu-id="b3515-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3515-128">The following table shows the properties that are required when you create the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

|<span data-ttu-id="b3515-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3515-129">Property</span></span>|<span data-ttu-id="b3515-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3515-130">Type</span></span>|<span data-ttu-id="b3515-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3515-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3515-132">id</span><span class="sxs-lookup"><span data-stu-id="b3515-132">id</span></span>|<span data-ttu-id="b3515-133">String</span><span class="sxs-lookup"><span data-stu-id="b3515-133">String</span></span>|<span data-ttu-id="b3515-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b3515-134">Key of the entity.</span></span> <span data-ttu-id="b3515-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b3515-136">displayName</span></span>|<span data-ttu-id="b3515-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3515-137">String</span></span>|<span data-ttu-id="b3515-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b3515-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b3515-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-140">description</span><span class="sxs-lookup"><span data-stu-id="b3515-140">description</span></span>|<span data-ttu-id="b3515-141">String</span><span class="sxs-lookup"><span data-stu-id="b3515-141">String</span></span>|<span data-ttu-id="b3515-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b3515-142">The description of the app.</span></span> <span data-ttu-id="b3515-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-144">publicador</span><span class="sxs-lookup"><span data-stu-id="b3515-144">publisher</span></span>|<span data-ttu-id="b3515-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3515-145">String</span></span>|<span data-ttu-id="b3515-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b3515-146">The publisher of the app.</span></span> <span data-ttu-id="b3515-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b3515-148">largeIcon</span></span>|[<span data-ttu-id="b3515-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b3515-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b3515-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b3515-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b3515-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3515-152">createdDateTime</span></span>|<span data-ttu-id="b3515-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3515-153">DateTimeOffset</span></span>|<span data-ttu-id="b3515-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b3515-154">The date and time the app was created.</span></span> <span data-ttu-id="b3515-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3515-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b3515-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3515-157">DateTimeOffset</span></span>|<span data-ttu-id="b3515-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b3515-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b3515-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b3515-160">isFeatured</span></span>|<span data-ttu-id="b3515-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3515-161">Boolean</span></span>|<span data-ttu-id="b3515-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b3515-163">privacyInformationUrl</span></span>|<span data-ttu-id="b3515-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3515-164">String</span></span>|<span data-ttu-id="b3515-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b3515-165">The privacy statement Url.</span></span> <span data-ttu-id="b3515-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b3515-167">informationUrl</span></span>|<span data-ttu-id="b3515-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3515-168">String</span></span>|<span data-ttu-id="b3515-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b3515-169">The more information Url.</span></span> <span data-ttu-id="b3515-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-171">owner</span><span class="sxs-lookup"><span data-stu-id="b3515-171">owner</span></span>|<span data-ttu-id="b3515-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3515-172">String</span></span>|<span data-ttu-id="b3515-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b3515-173">The owner of the app.</span></span> <span data-ttu-id="b3515-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-175">developer</span><span class="sxs-lookup"><span data-stu-id="b3515-175">developer</span></span>|<span data-ttu-id="b3515-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3515-176">String</span></span>|<span data-ttu-id="b3515-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b3515-177">The developer of the app.</span></span> <span data-ttu-id="b3515-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-179">notes</span><span class="sxs-lookup"><span data-stu-id="b3515-179">notes</span></span>|<span data-ttu-id="b3515-180">String</span><span class="sxs-lookup"><span data-stu-id="b3515-180">String</span></span>|<span data-ttu-id="b3515-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b3515-181">Notes for the app.</span></span> <span data-ttu-id="b3515-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b3515-183">uploadState</span></span>|<span data-ttu-id="b3515-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b3515-184">Int32</span></span>|<span data-ttu-id="b3515-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="b3515-185">The upload state.</span></span> <span data-ttu-id="b3515-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b3515-187">publishingState</span></span>|[<span data-ttu-id="b3515-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b3515-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b3515-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b3515-189">The publishing state for the app.</span></span> <span data-ttu-id="b3515-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b3515-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b3515-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3515-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b3515-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b3515-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b3515-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b3515-193">isAssigned</span></span>|<span data-ttu-id="b3515-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3515-194">Boolean</span></span>|<span data-ttu-id="b3515-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="b3515-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b3515-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3515-197">roleScopeTagIds</span></span>|<span data-ttu-id="b3515-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b3515-198">String collection</span></span>|<span data-ttu-id="b3515-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b3515-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b3515-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b3515-201">dependentAppCount</span></span>|<span data-ttu-id="b3515-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b3515-202">Int32</span></span>|<span data-ttu-id="b3515-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="b3515-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b3515-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3515-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b3515-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b3515-205">appStoreUrl</span></span>|<span data-ttu-id="b3515-206">String</span><span class="sxs-lookup"><span data-stu-id="b3515-206">String</span></span>|<span data-ttu-id="b3515-207">A URL da loja de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="b3515-207">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="b3515-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3515-208">Response</span></span>
<span data-ttu-id="b3515-209">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3515-209">If successful, this method returns a `200 OK` response code and an updated [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3515-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3515-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3515-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3515-211">Request</span></span>
<span data-ttu-id="b3515-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3515-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3515-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3515-213">Response</span></span>
<span data-ttu-id="b3515-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3515-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





