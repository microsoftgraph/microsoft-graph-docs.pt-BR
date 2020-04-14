---
title: Criar webApp
description: Cria um novo objeto webApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6461c25ce993791de33cba3eed11de8c456a1293
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43409620"
---
# <a name="create-webapp"></a><span data-ttu-id="20258-103">Criar webApp</span><span class="sxs-lookup"><span data-stu-id="20258-103">Create webApp</span></span>

<span data-ttu-id="20258-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20258-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20258-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20258-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20258-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20258-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20258-107">Cria um novo objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="20258-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20258-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20258-108">Prerequisites</span></span>
<span data-ttu-id="20258-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20258-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20258-111">Permission type</span></span>|<span data-ttu-id="20258-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20258-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20258-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20258-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20258-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20258-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20258-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20258-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20258-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20258-116">Not supported.</span></span>|
|<span data-ttu-id="20258-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20258-117">Application</span></span>|<span data-ttu-id="20258-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20258-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20258-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20258-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="20258-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20258-120">Request headers</span></span>
|<span data-ttu-id="20258-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20258-121">Header</span></span>|<span data-ttu-id="20258-122">Valor</span><span class="sxs-lookup"><span data-stu-id="20258-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20258-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20258-123">Authorization</span></span>|<span data-ttu-id="20258-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20258-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20258-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20258-125">Accept</span></span>|<span data-ttu-id="20258-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20258-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20258-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20258-127">Request body</span></span>
<span data-ttu-id="20258-128">No corpo da solicitação, forneça uma representação JSON do objeto webApp.</span><span class="sxs-lookup"><span data-stu-id="20258-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="20258-129">A tabela a seguir mostra as propriedades obrigatórias ao criar o webApp.</span><span class="sxs-lookup"><span data-stu-id="20258-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="20258-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20258-130">Property</span></span>|<span data-ttu-id="20258-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="20258-131">Type</span></span>|<span data-ttu-id="20258-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="20258-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20258-133">id</span><span class="sxs-lookup"><span data-stu-id="20258-133">id</span></span>|<span data-ttu-id="20258-134">String</span><span class="sxs-lookup"><span data-stu-id="20258-134">String</span></span>|<span data-ttu-id="20258-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="20258-135">Key of the entity.</span></span> <span data-ttu-id="20258-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-137">displayName</span><span class="sxs-lookup"><span data-stu-id="20258-137">displayName</span></span>|<span data-ttu-id="20258-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20258-138">String</span></span>|<span data-ttu-id="20258-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="20258-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="20258-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-141">description</span><span class="sxs-lookup"><span data-stu-id="20258-141">description</span></span>|<span data-ttu-id="20258-142">String</span><span class="sxs-lookup"><span data-stu-id="20258-142">String</span></span>|<span data-ttu-id="20258-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="20258-143">The description of the app.</span></span> <span data-ttu-id="20258-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-145">publicador</span><span class="sxs-lookup"><span data-stu-id="20258-145">publisher</span></span>|<span data-ttu-id="20258-146">String</span><span class="sxs-lookup"><span data-stu-id="20258-146">String</span></span>|<span data-ttu-id="20258-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="20258-147">The publisher of the app.</span></span> <span data-ttu-id="20258-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="20258-149">largeIcon</span></span>|[<span data-ttu-id="20258-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="20258-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="20258-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="20258-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="20258-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20258-153">createdDateTime</span></span>|<span data-ttu-id="20258-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20258-154">DateTimeOffset</span></span>|<span data-ttu-id="20258-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="20258-155">The date and time the app was created.</span></span> <span data-ttu-id="20258-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20258-157">lastModifiedDateTime</span></span>|<span data-ttu-id="20258-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20258-158">DateTimeOffset</span></span>|<span data-ttu-id="20258-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="20258-159">The date and time the app was last modified.</span></span> <span data-ttu-id="20258-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="20258-161">isFeatured</span></span>|<span data-ttu-id="20258-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="20258-162">Boolean</span></span>|<span data-ttu-id="20258-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="20258-164">privacyInformationUrl</span></span>|<span data-ttu-id="20258-165">String</span><span class="sxs-lookup"><span data-stu-id="20258-165">String</span></span>|<span data-ttu-id="20258-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="20258-166">The privacy statement Url.</span></span> <span data-ttu-id="20258-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="20258-168">informationUrl</span></span>|<span data-ttu-id="20258-169">String</span><span class="sxs-lookup"><span data-stu-id="20258-169">String</span></span>|<span data-ttu-id="20258-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="20258-170">The more information Url.</span></span> <span data-ttu-id="20258-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-172">owner</span><span class="sxs-lookup"><span data-stu-id="20258-172">owner</span></span>|<span data-ttu-id="20258-173">String</span><span class="sxs-lookup"><span data-stu-id="20258-173">String</span></span>|<span data-ttu-id="20258-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="20258-174">The owner of the app.</span></span> <span data-ttu-id="20258-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-176">developer</span><span class="sxs-lookup"><span data-stu-id="20258-176">developer</span></span>|<span data-ttu-id="20258-177">String</span><span class="sxs-lookup"><span data-stu-id="20258-177">String</span></span>|<span data-ttu-id="20258-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="20258-178">The developer of the app.</span></span> <span data-ttu-id="20258-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-180">notes</span><span class="sxs-lookup"><span data-stu-id="20258-180">notes</span></span>|<span data-ttu-id="20258-181">String</span><span class="sxs-lookup"><span data-stu-id="20258-181">String</span></span>|<span data-ttu-id="20258-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="20258-182">Notes for the app.</span></span> <span data-ttu-id="20258-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="20258-184">uploadState</span></span>|<span data-ttu-id="20258-185">Int32</span><span class="sxs-lookup"><span data-stu-id="20258-185">Int32</span></span>|<span data-ttu-id="20258-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="20258-186">The upload state.</span></span> <span data-ttu-id="20258-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="20258-188">publishingState</span></span>|[<span data-ttu-id="20258-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="20258-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="20258-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="20258-190">The publishing state for the app.</span></span> <span data-ttu-id="20258-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="20258-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="20258-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20258-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="20258-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="20258-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="20258-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="20258-194">isAssigned</span></span>|<span data-ttu-id="20258-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="20258-195">Boolean</span></span>|<span data-ttu-id="20258-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="20258-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="20258-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20258-198">roleScopeTagIds</span></span>|<span data-ttu-id="20258-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="20258-199">String collection</span></span>|<span data-ttu-id="20258-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="20258-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="20258-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="20258-202">dependentAppCount</span></span>|<span data-ttu-id="20258-203">Int32</span><span class="sxs-lookup"><span data-stu-id="20258-203">Int32</span></span>|<span data-ttu-id="20258-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="20258-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="20258-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="20258-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20258-206">appUrl</span><span class="sxs-lookup"><span data-stu-id="20258-206">appUrl</span></span>|<span data-ttu-id="20258-207">String</span><span class="sxs-lookup"><span data-stu-id="20258-207">String</span></span>|<span data-ttu-id="20258-208">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="20258-208">The web app URL.</span></span>|
|<span data-ttu-id="20258-209">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="20258-209">useManagedBrowser</span></span>|<span data-ttu-id="20258-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="20258-210">Boolean</span></span>|<span data-ttu-id="20258-211">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="20258-211">Whether or not to use managed browser.</span></span> <span data-ttu-id="20258-212">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="20258-212">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="20258-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="20258-213">Response</span></span>
<span data-ttu-id="20258-214">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20258-214">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20258-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20258-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="20258-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20258-216">Request</span></span>
<span data-ttu-id="20258-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20258-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="20258-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="20258-218">Response</span></span>
<span data-ttu-id="20258-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20258-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



