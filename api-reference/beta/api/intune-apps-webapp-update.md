---
title: Atualizar webApp
description: Atualiza as propriedades de um objeto webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c685b595fe528a5fbc5cd5a10c007a0dea4564ca
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973402"
---
# <a name="update-webapp"></a><span data-ttu-id="08644-103">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="08644-103">Update webApp</span></span>

> <span data-ttu-id="08644-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08644-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08644-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08644-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08644-106">Atualiza as propriedades de um objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="08644-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08644-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08644-107">Prerequisites</span></span>
<span data-ttu-id="08644-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08644-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08644-110">Permission type</span></span>|<span data-ttu-id="08644-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08644-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08644-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08644-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08644-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08644-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="08644-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08644-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08644-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08644-115">Not supported.</span></span>|
|<span data-ttu-id="08644-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08644-116">Application</span></span>|<span data-ttu-id="08644-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08644-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08644-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08644-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="08644-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08644-119">Request headers</span></span>
|<span data-ttu-id="08644-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08644-120">Header</span></span>|<span data-ttu-id="08644-121">Valor</span><span class="sxs-lookup"><span data-stu-id="08644-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08644-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="08644-122">Authorization</span></span>|<span data-ttu-id="08644-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08644-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08644-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08644-124">Accept</span></span>|<span data-ttu-id="08644-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08644-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08644-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08644-126">Request body</span></span>
<span data-ttu-id="08644-127">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="08644-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="08644-128">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="08644-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="08644-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08644-129">Property</span></span>|<span data-ttu-id="08644-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="08644-130">Type</span></span>|<span data-ttu-id="08644-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="08644-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08644-132">id</span><span class="sxs-lookup"><span data-stu-id="08644-132">id</span></span>|<span data-ttu-id="08644-133">String</span><span class="sxs-lookup"><span data-stu-id="08644-133">String</span></span>|<span data-ttu-id="08644-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="08644-134">Key of the entity.</span></span> <span data-ttu-id="08644-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-136">displayName</span><span class="sxs-lookup"><span data-stu-id="08644-136">displayName</span></span>|<span data-ttu-id="08644-137">String</span><span class="sxs-lookup"><span data-stu-id="08644-137">String</span></span>|<span data-ttu-id="08644-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="08644-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="08644-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-140">descrição</span><span class="sxs-lookup"><span data-stu-id="08644-140">description</span></span>|<span data-ttu-id="08644-141">String</span><span class="sxs-lookup"><span data-stu-id="08644-141">String</span></span>|<span data-ttu-id="08644-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08644-142">The description of the app.</span></span> <span data-ttu-id="08644-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-144">publicador</span><span class="sxs-lookup"><span data-stu-id="08644-144">publisher</span></span>|<span data-ttu-id="08644-145">String</span><span class="sxs-lookup"><span data-stu-id="08644-145">String</span></span>|<span data-ttu-id="08644-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08644-146">The publisher of the app.</span></span> <span data-ttu-id="08644-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="08644-148">largeIcon</span></span>|[<span data-ttu-id="08644-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="08644-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="08644-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="08644-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="08644-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08644-152">createdDateTime</span></span>|<span data-ttu-id="08644-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08644-153">DateTimeOffset</span></span>|<span data-ttu-id="08644-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08644-154">The date and time the app was created.</span></span> <span data-ttu-id="08644-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08644-156">lastModifiedDateTime</span></span>|<span data-ttu-id="08644-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08644-157">DateTimeOffset</span></span>|<span data-ttu-id="08644-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="08644-158">The date and time the app was last modified.</span></span> <span data-ttu-id="08644-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="08644-160">isFeatured</span></span>|<span data-ttu-id="08644-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="08644-161">Boolean</span></span>|<span data-ttu-id="08644-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="08644-163">privacyInformationUrl</span></span>|<span data-ttu-id="08644-164">String</span><span class="sxs-lookup"><span data-stu-id="08644-164">String</span></span>|<span data-ttu-id="08644-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="08644-165">The privacy statement Url.</span></span> <span data-ttu-id="08644-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="08644-167">informationUrl</span></span>|<span data-ttu-id="08644-168">String</span><span class="sxs-lookup"><span data-stu-id="08644-168">String</span></span>|<span data-ttu-id="08644-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="08644-169">The more information Url.</span></span> <span data-ttu-id="08644-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-171">owner</span><span class="sxs-lookup"><span data-stu-id="08644-171">owner</span></span>|<span data-ttu-id="08644-172">String</span><span class="sxs-lookup"><span data-stu-id="08644-172">String</span></span>|<span data-ttu-id="08644-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="08644-173">The owner of the app.</span></span> <span data-ttu-id="08644-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-175">developer</span><span class="sxs-lookup"><span data-stu-id="08644-175">developer</span></span>|<span data-ttu-id="08644-176">String</span><span class="sxs-lookup"><span data-stu-id="08644-176">String</span></span>|<span data-ttu-id="08644-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08644-177">The developer of the app.</span></span> <span data-ttu-id="08644-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-179">notes</span><span class="sxs-lookup"><span data-stu-id="08644-179">notes</span></span>|<span data-ttu-id="08644-180">String</span><span class="sxs-lookup"><span data-stu-id="08644-180">String</span></span>|<span data-ttu-id="08644-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08644-181">Notes for the app.</span></span> <span data-ttu-id="08644-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="08644-183">uploadState</span></span>|<span data-ttu-id="08644-184">Int32</span><span class="sxs-lookup"><span data-stu-id="08644-184">Int32</span></span>|<span data-ttu-id="08644-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="08644-185">The upload state.</span></span> <span data-ttu-id="08644-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="08644-187">publishingState</span></span>|[<span data-ttu-id="08644-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="08644-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="08644-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08644-189">The publishing state for the app.</span></span> <span data-ttu-id="08644-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="08644-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="08644-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="08644-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="08644-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="08644-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="08644-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="08644-193">isAssigned</span></span>|<span data-ttu-id="08644-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="08644-194">Boolean</span></span>|<span data-ttu-id="08644-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="08644-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="08644-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08644-197">roleScopeTagIds</span></span>|<span data-ttu-id="08644-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="08644-198">String collection</span></span>|<span data-ttu-id="08644-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="08644-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="08644-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="08644-201">dependentAppCount</span></span>|<span data-ttu-id="08644-202">Int32</span><span class="sxs-lookup"><span data-stu-id="08644-202">Int32</span></span>|<span data-ttu-id="08644-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="08644-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="08644-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="08644-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="08644-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="08644-205">appUrl</span></span>|<span data-ttu-id="08644-206">String</span><span class="sxs-lookup"><span data-stu-id="08644-206">String</span></span>|<span data-ttu-id="08644-207">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="08644-207">The web app URL.</span></span>|
|<span data-ttu-id="08644-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="08644-208">useManagedBrowser</span></span>|<span data-ttu-id="08644-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="08644-209">Boolean</span></span>|<span data-ttu-id="08644-210">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="08644-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="08644-211">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="08644-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="08644-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="08644-212">Response</span></span>
<span data-ttu-id="08644-213">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune-apps-webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08644-213">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08644-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08644-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="08644-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08644-215">Request</span></span>
<span data-ttu-id="08644-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08644-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 779

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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="08644-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="08644-217">Response</span></span>
<span data-ttu-id="08644-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08644-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 951

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```





