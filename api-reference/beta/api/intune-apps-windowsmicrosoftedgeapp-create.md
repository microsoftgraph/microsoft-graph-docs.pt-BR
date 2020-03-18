---
title: Criar windowsMicrosoftEdgeApp
description: Criar um novo objeto windowsMicrosoftEdgeApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86cc901ce6541c9d97dac55b6580575b6fa8f415
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760918"
---
# <a name="create-windowsmicrosoftedgeapp"></a><span data-ttu-id="de82d-103">Criar windowsMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="de82d-103">Create windowsMicrosoftEdgeApp</span></span>

> <span data-ttu-id="de82d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de82d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de82d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de82d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de82d-106">Criar um novo objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="de82d-106">Create a new [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de82d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de82d-107">Prerequisites</span></span>
<span data-ttu-id="de82d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de82d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de82d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de82d-110">Permission type</span></span>|<span data-ttu-id="de82d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de82d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de82d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de82d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de82d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de82d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de82d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de82d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de82d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de82d-115">Not supported.</span></span>|
|<span data-ttu-id="de82d-116">Application</span><span class="sxs-lookup"><span data-stu-id="de82d-116">Application</span></span>|<span data-ttu-id="de82d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de82d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de82d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de82d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="de82d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de82d-119">Request headers</span></span>
|<span data-ttu-id="de82d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de82d-120">Header</span></span>|<span data-ttu-id="de82d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="de82d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de82d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="de82d-122">Authorization</span></span>|<span data-ttu-id="de82d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de82d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de82d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de82d-124">Accept</span></span>|<span data-ttu-id="de82d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de82d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de82d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de82d-126">Request body</span></span>
<span data-ttu-id="de82d-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="de82d-127">In the request body, supply a JSON representation for the windowsMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="de82d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="de82d-128">The following table shows the properties that are required when you create the windowsMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="de82d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de82d-129">Property</span></span>|<span data-ttu-id="de82d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="de82d-130">Type</span></span>|<span data-ttu-id="de82d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="de82d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de82d-132">id</span><span class="sxs-lookup"><span data-stu-id="de82d-132">id</span></span>|<span data-ttu-id="de82d-133">String</span><span class="sxs-lookup"><span data-stu-id="de82d-133">String</span></span>|<span data-ttu-id="de82d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de82d-134">Key of the entity.</span></span> <span data-ttu-id="de82d-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="de82d-136">displayName</span></span>|<span data-ttu-id="de82d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de82d-137">String</span></span>|<span data-ttu-id="de82d-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="de82d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="de82d-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-140">description</span><span class="sxs-lookup"><span data-stu-id="de82d-140">description</span></span>|<span data-ttu-id="de82d-141">String</span><span class="sxs-lookup"><span data-stu-id="de82d-141">String</span></span>|<span data-ttu-id="de82d-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de82d-142">The description of the app.</span></span> <span data-ttu-id="de82d-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-144">publicador</span><span class="sxs-lookup"><span data-stu-id="de82d-144">publisher</span></span>|<span data-ttu-id="de82d-145">String</span><span class="sxs-lookup"><span data-stu-id="de82d-145">String</span></span>|<span data-ttu-id="de82d-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de82d-146">The publisher of the app.</span></span> <span data-ttu-id="de82d-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="de82d-148">largeIcon</span></span>|[<span data-ttu-id="de82d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="de82d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="de82d-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="de82d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="de82d-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de82d-152">createdDateTime</span></span>|<span data-ttu-id="de82d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de82d-153">DateTimeOffset</span></span>|<span data-ttu-id="de82d-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de82d-154">The date and time the app was created.</span></span> <span data-ttu-id="de82d-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de82d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="de82d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de82d-157">DateTimeOffset</span></span>|<span data-ttu-id="de82d-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="de82d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="de82d-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="de82d-160">isFeatured</span></span>|<span data-ttu-id="de82d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="de82d-161">Boolean</span></span>|<span data-ttu-id="de82d-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="de82d-163">privacyInformationUrl</span></span>|<span data-ttu-id="de82d-164">String</span><span class="sxs-lookup"><span data-stu-id="de82d-164">String</span></span>|<span data-ttu-id="de82d-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="de82d-165">The privacy statement Url.</span></span> <span data-ttu-id="de82d-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="de82d-167">informationUrl</span></span>|<span data-ttu-id="de82d-168">String</span><span class="sxs-lookup"><span data-stu-id="de82d-168">String</span></span>|<span data-ttu-id="de82d-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="de82d-169">The more information Url.</span></span> <span data-ttu-id="de82d-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-171">owner</span><span class="sxs-lookup"><span data-stu-id="de82d-171">owner</span></span>|<span data-ttu-id="de82d-172">String</span><span class="sxs-lookup"><span data-stu-id="de82d-172">String</span></span>|<span data-ttu-id="de82d-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="de82d-173">The owner of the app.</span></span> <span data-ttu-id="de82d-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-175">developer</span><span class="sxs-lookup"><span data-stu-id="de82d-175">developer</span></span>|<span data-ttu-id="de82d-176">String</span><span class="sxs-lookup"><span data-stu-id="de82d-176">String</span></span>|<span data-ttu-id="de82d-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de82d-177">The developer of the app.</span></span> <span data-ttu-id="de82d-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-179">notes</span><span class="sxs-lookup"><span data-stu-id="de82d-179">notes</span></span>|<span data-ttu-id="de82d-180">String</span><span class="sxs-lookup"><span data-stu-id="de82d-180">String</span></span>|<span data-ttu-id="de82d-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de82d-181">Notes for the app.</span></span> <span data-ttu-id="de82d-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="de82d-183">uploadState</span></span>|<span data-ttu-id="de82d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="de82d-184">Int32</span></span>|<span data-ttu-id="de82d-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="de82d-185">The upload state.</span></span> <span data-ttu-id="de82d-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="de82d-187">publishingState</span></span>|[<span data-ttu-id="de82d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="de82d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="de82d-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de82d-189">The publishing state for the app.</span></span> <span data-ttu-id="de82d-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="de82d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="de82d-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de82d-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="de82d-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="de82d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="de82d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="de82d-193">isAssigned</span></span>|<span data-ttu-id="de82d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="de82d-194">Boolean</span></span>|<span data-ttu-id="de82d-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="de82d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="de82d-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de82d-197">roleScopeTagIds</span></span>|<span data-ttu-id="de82d-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="de82d-198">String collection</span></span>|<span data-ttu-id="de82d-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="de82d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="de82d-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="de82d-201">dependentAppCount</span></span>|<span data-ttu-id="de82d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="de82d-202">Int32</span></span>|<span data-ttu-id="de82d-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="de82d-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="de82d-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de82d-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de82d-205">canal</span><span class="sxs-lookup"><span data-stu-id="de82d-205">channel</span></span>|[<span data-ttu-id="de82d-206">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="de82d-206">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="de82d-207">O canal a ser instalado nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="de82d-207">The channel to install on target devices.</span></span> <span data-ttu-id="de82d-208">Os valores possíveis são: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="de82d-208">Possible values are: `dev`, `beta`, `stable`.</span></span>|
|<span data-ttu-id="de82d-209">displayLanguageLocale</span><span class="sxs-lookup"><span data-stu-id="de82d-209">displayLanguageLocale</span></span>|<span data-ttu-id="de82d-210">String</span><span class="sxs-lookup"><span data-stu-id="de82d-210">String</span></span>|<span data-ttu-id="de82d-211">A localidade do idioma a ser usada quando o aplicativo de borda exibe texto para o usuário.</span><span class="sxs-lookup"><span data-stu-id="de82d-211">The language locale to use when the Edge app displays text to the user.</span></span>|



## <a name="response"></a><span data-ttu-id="de82d-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="de82d-212">Response</span></span>
<span data-ttu-id="de82d-213">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de82d-213">If successful, this method returns a `201 Created` response code and a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de82d-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de82d-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="de82d-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de82d-215">Request</span></span>
<span data-ttu-id="de82d-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de82d-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 805

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
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
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```

### <a name="response"></a><span data-ttu-id="de82d-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="de82d-217">Response</span></span>
<span data-ttu-id="de82d-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de82d-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
  "id": "a4d4a316-a316-a4d4-16a3-d4a416a3d4a4",
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
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```




