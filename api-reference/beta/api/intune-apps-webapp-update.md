---
title: Atualizar webApp
description: Atualiza as propriedades de um objeto webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a743938ef288d2c0480f3ed1029112ab9d1e02e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328813"
---
# <a name="update-webapp"></a><span data-ttu-id="d951e-103">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="d951e-103">Update webApp</span></span>

> <span data-ttu-id="d951e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d951e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d951e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d951e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d951e-106">Atualiza as propriedades de um objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="d951e-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d951e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d951e-107">Prerequisites</span></span>
<span data-ttu-id="d951e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d951e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d951e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d951e-110">Permission type</span></span>|<span data-ttu-id="d951e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d951e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d951e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d951e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d951e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d951e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d951e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d951e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d951e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d951e-115">Not supported.</span></span>|
|<span data-ttu-id="d951e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d951e-116">Application</span></span>|<span data-ttu-id="d951e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d951e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d951e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d951e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d951e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d951e-119">Request headers</span></span>
|<span data-ttu-id="d951e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d951e-120">Header</span></span>|<span data-ttu-id="d951e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d951e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d951e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d951e-122">Authorization</span></span>|<span data-ttu-id="d951e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d951e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d951e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d951e-124">Accept</span></span>|<span data-ttu-id="d951e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d951e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d951e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d951e-126">Request body</span></span>
<span data-ttu-id="d951e-127">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="d951e-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="d951e-128">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="d951e-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="d951e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d951e-129">Property</span></span>|<span data-ttu-id="d951e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d951e-130">Type</span></span>|<span data-ttu-id="d951e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d951e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d951e-132">id</span><span class="sxs-lookup"><span data-stu-id="d951e-132">id</span></span>|<span data-ttu-id="d951e-133">String</span><span class="sxs-lookup"><span data-stu-id="d951e-133">String</span></span>|<span data-ttu-id="d951e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d951e-134">Key of the entity.</span></span> <span data-ttu-id="d951e-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d951e-136">displayName</span></span>|<span data-ttu-id="d951e-137">String</span><span class="sxs-lookup"><span data-stu-id="d951e-137">String</span></span>|<span data-ttu-id="d951e-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d951e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d951e-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-140">descrição</span><span class="sxs-lookup"><span data-stu-id="d951e-140">description</span></span>|<span data-ttu-id="d951e-141">String</span><span class="sxs-lookup"><span data-stu-id="d951e-141">String</span></span>|<span data-ttu-id="d951e-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d951e-142">The description of the app.</span></span> <span data-ttu-id="d951e-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-144">publicador</span><span class="sxs-lookup"><span data-stu-id="d951e-144">publisher</span></span>|<span data-ttu-id="d951e-145">String</span><span class="sxs-lookup"><span data-stu-id="d951e-145">String</span></span>|<span data-ttu-id="d951e-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d951e-146">The publisher of the app.</span></span> <span data-ttu-id="d951e-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d951e-148">largeIcon</span></span>|[<span data-ttu-id="d951e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d951e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d951e-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d951e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d951e-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d951e-152">createdDateTime</span></span>|<span data-ttu-id="d951e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d951e-153">DateTimeOffset</span></span>|<span data-ttu-id="d951e-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d951e-154">The date and time the app was created.</span></span> <span data-ttu-id="d951e-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d951e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d951e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d951e-157">DateTimeOffset</span></span>|<span data-ttu-id="d951e-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d951e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d951e-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d951e-160">isFeatured</span></span>|<span data-ttu-id="d951e-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="d951e-161">Boolean</span></span>|<span data-ttu-id="d951e-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d951e-163">privacyInformationUrl</span></span>|<span data-ttu-id="d951e-164">String</span><span class="sxs-lookup"><span data-stu-id="d951e-164">String</span></span>|<span data-ttu-id="d951e-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d951e-165">The privacy statement Url.</span></span> <span data-ttu-id="d951e-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d951e-167">informationUrl</span></span>|<span data-ttu-id="d951e-168">String</span><span class="sxs-lookup"><span data-stu-id="d951e-168">String</span></span>|<span data-ttu-id="d951e-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d951e-169">The more information Url.</span></span> <span data-ttu-id="d951e-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-171">owner</span><span class="sxs-lookup"><span data-stu-id="d951e-171">owner</span></span>|<span data-ttu-id="d951e-172">String</span><span class="sxs-lookup"><span data-stu-id="d951e-172">String</span></span>|<span data-ttu-id="d951e-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d951e-173">The owner of the app.</span></span> <span data-ttu-id="d951e-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-175">developer</span><span class="sxs-lookup"><span data-stu-id="d951e-175">developer</span></span>|<span data-ttu-id="d951e-176">String</span><span class="sxs-lookup"><span data-stu-id="d951e-176">String</span></span>|<span data-ttu-id="d951e-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d951e-177">The developer of the app.</span></span> <span data-ttu-id="d951e-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-179">notes</span><span class="sxs-lookup"><span data-stu-id="d951e-179">notes</span></span>|<span data-ttu-id="d951e-180">String</span><span class="sxs-lookup"><span data-stu-id="d951e-180">String</span></span>|<span data-ttu-id="d951e-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d951e-181">Notes for the app.</span></span> <span data-ttu-id="d951e-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d951e-183">uploadState</span></span>|<span data-ttu-id="d951e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d951e-184">Int32</span></span>|<span data-ttu-id="d951e-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="d951e-185">The upload state.</span></span> <span data-ttu-id="d951e-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d951e-187">publishingState</span></span>|[<span data-ttu-id="d951e-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d951e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d951e-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d951e-189">The publishing state for the app.</span></span> <span data-ttu-id="d951e-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d951e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d951e-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d951e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d951e-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d951e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d951e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d951e-193">isAssigned</span></span>|<span data-ttu-id="d951e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d951e-194">Boolean</span></span>|<span data-ttu-id="d951e-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="d951e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d951e-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d951e-197">roleScopeTagIds</span></span>|<span data-ttu-id="d951e-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d951e-198">String collection</span></span>|<span data-ttu-id="d951e-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d951e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d951e-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d951e-201">dependentAppCount</span></span>|<span data-ttu-id="d951e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d951e-202">Int32</span></span>|<span data-ttu-id="d951e-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="d951e-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d951e-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d951e-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d951e-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="d951e-205">appUrl</span></span>|<span data-ttu-id="d951e-206">String</span><span class="sxs-lookup"><span data-stu-id="d951e-206">String</span></span>|<span data-ttu-id="d951e-207">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="d951e-207">The web app URL.</span></span>|
|<span data-ttu-id="d951e-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="d951e-208">useManagedBrowser</span></span>|<span data-ttu-id="d951e-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="d951e-209">Boolean</span></span>|<span data-ttu-id="d951e-210">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="d951e-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="d951e-211">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="d951e-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="d951e-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="d951e-212">Response</span></span>
<span data-ttu-id="d951e-213">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune-apps-webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d951e-213">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d951e-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d951e-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="d951e-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d951e-215">Request</span></span>
<span data-ttu-id="d951e-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d951e-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d951e-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="d951e-217">Response</span></span>
<span data-ttu-id="d951e-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d951e-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






