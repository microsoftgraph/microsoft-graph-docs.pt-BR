---
title: Criar windowsMicrosoftEdgeApp
description: Criar um novo objeto windowsMicrosoftEdgeApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41dbf19434aa39f5d8d11b02ec5c5212c36fd248
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444816"
---
# <a name="create-windowsmicrosoftedgeapp"></a><span data-ttu-id="40768-103">Criar windowsMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="40768-103">Create windowsMicrosoftEdgeApp</span></span>

<span data-ttu-id="40768-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="40768-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40768-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40768-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40768-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40768-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40768-107">Criar um novo objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="40768-107">Create a new [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40768-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40768-108">Prerequisites</span></span>
<span data-ttu-id="40768-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40768-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40768-111">Permission type</span></span>|<span data-ttu-id="40768-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40768-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40768-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40768-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40768-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40768-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40768-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40768-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40768-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40768-116">Not supported.</span></span>|
|<span data-ttu-id="40768-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40768-117">Application</span></span>|<span data-ttu-id="40768-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40768-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40768-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40768-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="40768-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40768-120">Request headers</span></span>
|<span data-ttu-id="40768-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40768-121">Header</span></span>|<span data-ttu-id="40768-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40768-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40768-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40768-123">Authorization</span></span>|<span data-ttu-id="40768-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40768-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40768-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40768-125">Accept</span></span>|<span data-ttu-id="40768-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40768-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40768-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40768-127">Request body</span></span>
<span data-ttu-id="40768-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="40768-128">In the request body, supply a JSON representation for the windowsMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="40768-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="40768-129">The following table shows the properties that are required when you create the windowsMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="40768-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40768-130">Property</span></span>|<span data-ttu-id="40768-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="40768-131">Type</span></span>|<span data-ttu-id="40768-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="40768-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40768-133">id</span><span class="sxs-lookup"><span data-stu-id="40768-133">id</span></span>|<span data-ttu-id="40768-134">String</span><span class="sxs-lookup"><span data-stu-id="40768-134">String</span></span>|<span data-ttu-id="40768-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="40768-135">Key of the entity.</span></span> <span data-ttu-id="40768-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-137">displayName</span><span class="sxs-lookup"><span data-stu-id="40768-137">displayName</span></span>|<span data-ttu-id="40768-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40768-138">String</span></span>|<span data-ttu-id="40768-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="40768-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="40768-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-141">description</span><span class="sxs-lookup"><span data-stu-id="40768-141">description</span></span>|<span data-ttu-id="40768-142">String</span><span class="sxs-lookup"><span data-stu-id="40768-142">String</span></span>|<span data-ttu-id="40768-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40768-143">The description of the app.</span></span> <span data-ttu-id="40768-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-145">publicador</span><span class="sxs-lookup"><span data-stu-id="40768-145">publisher</span></span>|<span data-ttu-id="40768-146">String</span><span class="sxs-lookup"><span data-stu-id="40768-146">String</span></span>|<span data-ttu-id="40768-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40768-147">The publisher of the app.</span></span> <span data-ttu-id="40768-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="40768-149">largeIcon</span></span>|[<span data-ttu-id="40768-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="40768-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="40768-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="40768-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="40768-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40768-153">createdDateTime</span></span>|<span data-ttu-id="40768-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40768-154">DateTimeOffset</span></span>|<span data-ttu-id="40768-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40768-155">The date and time the app was created.</span></span> <span data-ttu-id="40768-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40768-157">lastModifiedDateTime</span></span>|<span data-ttu-id="40768-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40768-158">DateTimeOffset</span></span>|<span data-ttu-id="40768-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="40768-159">The date and time the app was last modified.</span></span> <span data-ttu-id="40768-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="40768-161">isFeatured</span></span>|<span data-ttu-id="40768-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="40768-162">Boolean</span></span>|<span data-ttu-id="40768-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="40768-164">privacyInformationUrl</span></span>|<span data-ttu-id="40768-165">String</span><span class="sxs-lookup"><span data-stu-id="40768-165">String</span></span>|<span data-ttu-id="40768-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="40768-166">The privacy statement Url.</span></span> <span data-ttu-id="40768-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="40768-168">informationUrl</span></span>|<span data-ttu-id="40768-169">String</span><span class="sxs-lookup"><span data-stu-id="40768-169">String</span></span>|<span data-ttu-id="40768-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="40768-170">The more information Url.</span></span> <span data-ttu-id="40768-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-172">owner</span><span class="sxs-lookup"><span data-stu-id="40768-172">owner</span></span>|<span data-ttu-id="40768-173">String</span><span class="sxs-lookup"><span data-stu-id="40768-173">String</span></span>|<span data-ttu-id="40768-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="40768-174">The owner of the app.</span></span> <span data-ttu-id="40768-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-176">developer</span><span class="sxs-lookup"><span data-stu-id="40768-176">developer</span></span>|<span data-ttu-id="40768-177">String</span><span class="sxs-lookup"><span data-stu-id="40768-177">String</span></span>|<span data-ttu-id="40768-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40768-178">The developer of the app.</span></span> <span data-ttu-id="40768-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-180">notes</span><span class="sxs-lookup"><span data-stu-id="40768-180">notes</span></span>|<span data-ttu-id="40768-181">String</span><span class="sxs-lookup"><span data-stu-id="40768-181">String</span></span>|<span data-ttu-id="40768-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40768-182">Notes for the app.</span></span> <span data-ttu-id="40768-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="40768-184">uploadState</span></span>|<span data-ttu-id="40768-185">Int32</span><span class="sxs-lookup"><span data-stu-id="40768-185">Int32</span></span>|<span data-ttu-id="40768-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="40768-186">The upload state.</span></span> <span data-ttu-id="40768-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="40768-188">publishingState</span></span>|[<span data-ttu-id="40768-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="40768-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="40768-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40768-190">The publishing state for the app.</span></span> <span data-ttu-id="40768-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="40768-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="40768-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40768-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="40768-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="40768-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="40768-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="40768-194">isAssigned</span></span>|<span data-ttu-id="40768-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="40768-195">Boolean</span></span>|<span data-ttu-id="40768-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="40768-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="40768-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="40768-198">roleScopeTagIds</span></span>|<span data-ttu-id="40768-199">String collection</span><span class="sxs-lookup"><span data-stu-id="40768-199">String collection</span></span>|<span data-ttu-id="40768-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="40768-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="40768-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="40768-202">dependentAppCount</span></span>|<span data-ttu-id="40768-203">Int32</span><span class="sxs-lookup"><span data-stu-id="40768-203">Int32</span></span>|<span data-ttu-id="40768-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="40768-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="40768-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40768-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="40768-206">canal</span><span class="sxs-lookup"><span data-stu-id="40768-206">channel</span></span>|[<span data-ttu-id="40768-207">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="40768-207">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="40768-208">O canal a ser instalado nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="40768-208">The channel to install on target devices.</span></span> <span data-ttu-id="40768-209">Os valores possíveis são: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="40768-209">Possible values are: `dev`, `beta`, `stable`.</span></span>|
|<span data-ttu-id="40768-210">displayLanguageLocale</span><span class="sxs-lookup"><span data-stu-id="40768-210">displayLanguageLocale</span></span>|<span data-ttu-id="40768-211">String</span><span class="sxs-lookup"><span data-stu-id="40768-211">String</span></span>|<span data-ttu-id="40768-212">A localidade do idioma a ser usada quando o aplicativo de borda exibe texto para o usuário.</span><span class="sxs-lookup"><span data-stu-id="40768-212">The language locale to use when the Edge app displays text to the user.</span></span>|



## <a name="response"></a><span data-ttu-id="40768-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="40768-213">Response</span></span>
<span data-ttu-id="40768-214">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40768-214">If successful, this method returns a `201 Created` response code and a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40768-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40768-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="40768-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40768-216">Request</span></span>
<span data-ttu-id="40768-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40768-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="40768-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="40768-218">Response</span></span>
<span data-ttu-id="40768-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40768-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





