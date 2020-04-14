---
title: Criar windowsMicrosoftEdgeApp
description: Criar um novo objeto windowsMicrosoftEdgeApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3988829f209079b7eedda5d28b95de6b56682fbc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393683"
---
# <a name="create-windowsmicrosoftedgeapp"></a><span data-ttu-id="2f981-103">Criar windowsMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="2f981-103">Create windowsMicrosoftEdgeApp</span></span>

<span data-ttu-id="2f981-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f981-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f981-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f981-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f981-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f981-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f981-107">Criar um novo objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2f981-107">Create a new [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f981-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f981-108">Prerequisites</span></span>
<span data-ttu-id="2f981-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f981-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f981-111">Permission type</span></span>|<span data-ttu-id="2f981-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f981-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f981-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f981-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f981-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f981-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f981-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f981-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f981-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f981-116">Not supported.</span></span>|
|<span data-ttu-id="2f981-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f981-117">Application</span></span>|<span data-ttu-id="2f981-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f981-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f981-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f981-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2f981-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f981-120">Request headers</span></span>
|<span data-ttu-id="2f981-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f981-121">Header</span></span>|<span data-ttu-id="2f981-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f981-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f981-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f981-123">Authorization</span></span>|<span data-ttu-id="2f981-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f981-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f981-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f981-125">Accept</span></span>|<span data-ttu-id="2f981-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f981-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f981-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f981-127">Request body</span></span>
<span data-ttu-id="2f981-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="2f981-128">In the request body, supply a JSON representation for the windowsMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="2f981-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="2f981-129">The following table shows the properties that are required when you create the windowsMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="2f981-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f981-130">Property</span></span>|<span data-ttu-id="2f981-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f981-131">Type</span></span>|<span data-ttu-id="2f981-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f981-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f981-133">id</span><span class="sxs-lookup"><span data-stu-id="2f981-133">id</span></span>|<span data-ttu-id="2f981-134">String</span><span class="sxs-lookup"><span data-stu-id="2f981-134">String</span></span>|<span data-ttu-id="2f981-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f981-135">Key of the entity.</span></span> <span data-ttu-id="2f981-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2f981-137">displayName</span></span>|<span data-ttu-id="2f981-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f981-138">String</span></span>|<span data-ttu-id="2f981-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2f981-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2f981-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-141">description</span><span class="sxs-lookup"><span data-stu-id="2f981-141">description</span></span>|<span data-ttu-id="2f981-142">String</span><span class="sxs-lookup"><span data-stu-id="2f981-142">String</span></span>|<span data-ttu-id="2f981-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f981-143">The description of the app.</span></span> <span data-ttu-id="2f981-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-145">publicador</span><span class="sxs-lookup"><span data-stu-id="2f981-145">publisher</span></span>|<span data-ttu-id="2f981-146">String</span><span class="sxs-lookup"><span data-stu-id="2f981-146">String</span></span>|<span data-ttu-id="2f981-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f981-147">The publisher of the app.</span></span> <span data-ttu-id="2f981-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2f981-149">largeIcon</span></span>|[<span data-ttu-id="2f981-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2f981-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2f981-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2f981-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2f981-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f981-153">createdDateTime</span></span>|<span data-ttu-id="2f981-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f981-154">DateTimeOffset</span></span>|<span data-ttu-id="2f981-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f981-155">The date and time the app was created.</span></span> <span data-ttu-id="2f981-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f981-157">lastModifiedDateTime</span></span>|<span data-ttu-id="2f981-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f981-158">DateTimeOffset</span></span>|<span data-ttu-id="2f981-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2f981-159">The date and time the app was last modified.</span></span> <span data-ttu-id="2f981-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2f981-161">isFeatured</span></span>|<span data-ttu-id="2f981-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f981-162">Boolean</span></span>|<span data-ttu-id="2f981-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2f981-164">privacyInformationUrl</span></span>|<span data-ttu-id="2f981-165">String</span><span class="sxs-lookup"><span data-stu-id="2f981-165">String</span></span>|<span data-ttu-id="2f981-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2f981-166">The privacy statement Url.</span></span> <span data-ttu-id="2f981-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2f981-168">informationUrl</span></span>|<span data-ttu-id="2f981-169">String</span><span class="sxs-lookup"><span data-stu-id="2f981-169">String</span></span>|<span data-ttu-id="2f981-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2f981-170">The more information Url.</span></span> <span data-ttu-id="2f981-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-172">owner</span><span class="sxs-lookup"><span data-stu-id="2f981-172">owner</span></span>|<span data-ttu-id="2f981-173">String</span><span class="sxs-lookup"><span data-stu-id="2f981-173">String</span></span>|<span data-ttu-id="2f981-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2f981-174">The owner of the app.</span></span> <span data-ttu-id="2f981-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-176">developer</span><span class="sxs-lookup"><span data-stu-id="2f981-176">developer</span></span>|<span data-ttu-id="2f981-177">String</span><span class="sxs-lookup"><span data-stu-id="2f981-177">String</span></span>|<span data-ttu-id="2f981-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f981-178">The developer of the app.</span></span> <span data-ttu-id="2f981-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-180">notes</span><span class="sxs-lookup"><span data-stu-id="2f981-180">notes</span></span>|<span data-ttu-id="2f981-181">String</span><span class="sxs-lookup"><span data-stu-id="2f981-181">String</span></span>|<span data-ttu-id="2f981-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f981-182">Notes for the app.</span></span> <span data-ttu-id="2f981-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="2f981-184">uploadState</span></span>|<span data-ttu-id="2f981-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2f981-185">Int32</span></span>|<span data-ttu-id="2f981-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="2f981-186">The upload state.</span></span> <span data-ttu-id="2f981-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="2f981-188">publishingState</span></span>|[<span data-ttu-id="2f981-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2f981-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2f981-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f981-190">The publishing state for the app.</span></span> <span data-ttu-id="2f981-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2f981-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2f981-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f981-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2f981-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2f981-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2f981-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2f981-194">isAssigned</span></span>|<span data-ttu-id="2f981-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f981-195">Boolean</span></span>|<span data-ttu-id="2f981-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="2f981-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2f981-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f981-198">roleScopeTagIds</span></span>|<span data-ttu-id="2f981-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="2f981-199">String collection</span></span>|<span data-ttu-id="2f981-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2f981-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2f981-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="2f981-202">dependentAppCount</span></span>|<span data-ttu-id="2f981-203">Int32</span><span class="sxs-lookup"><span data-stu-id="2f981-203">Int32</span></span>|<span data-ttu-id="2f981-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="2f981-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2f981-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f981-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2f981-206">canal</span><span class="sxs-lookup"><span data-stu-id="2f981-206">channel</span></span>|[<span data-ttu-id="2f981-207">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="2f981-207">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="2f981-208">O canal a ser instalado nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="2f981-208">The channel to install on target devices.</span></span> <span data-ttu-id="2f981-209">Os valores possíveis são: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="2f981-209">Possible values are: `dev`, `beta`, `stable`.</span></span>|
|<span data-ttu-id="2f981-210">displayLanguageLocale</span><span class="sxs-lookup"><span data-stu-id="2f981-210">displayLanguageLocale</span></span>|<span data-ttu-id="2f981-211">String</span><span class="sxs-lookup"><span data-stu-id="2f981-211">String</span></span>|<span data-ttu-id="2f981-212">A localidade do idioma a ser usada quando o aplicativo de borda exibe texto para o usuário.</span><span class="sxs-lookup"><span data-stu-id="2f981-212">The language locale to use when the Edge app displays text to the user.</span></span>|



## <a name="response"></a><span data-ttu-id="2f981-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f981-213">Response</span></span>
<span data-ttu-id="2f981-214">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f981-214">If successful, this method returns a `201 Created` response code and a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f981-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f981-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f981-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f981-216">Request</span></span>
<span data-ttu-id="2f981-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f981-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f981-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f981-218">Response</span></span>
<span data-ttu-id="2f981-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f981-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



