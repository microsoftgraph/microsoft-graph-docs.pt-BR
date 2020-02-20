---
title: Criar windowsMicrosoftEdgeApp
description: Criar um novo objeto windowsMicrosoftEdgeApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2fcac61ae162b8acf96fd6271d2fdcdb7fc6b654
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160309"
---
# <a name="create-windowsmicrosoftedgeapp"></a><span data-ttu-id="cb350-103">Criar windowsMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="cb350-103">Create windowsMicrosoftEdgeApp</span></span>

> <span data-ttu-id="cb350-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb350-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb350-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb350-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb350-106">Criar um novo objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="cb350-106">Create a new [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb350-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb350-107">Prerequisites</span></span>
<span data-ttu-id="cb350-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb350-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb350-110">Permission type</span></span>|<span data-ttu-id="cb350-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb350-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb350-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb350-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb350-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb350-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb350-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb350-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb350-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb350-115">Not supported.</span></span>|
|<span data-ttu-id="cb350-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb350-116">Application</span></span>|<span data-ttu-id="cb350-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb350-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb350-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb350-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cb350-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb350-119">Request headers</span></span>
|<span data-ttu-id="cb350-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb350-120">Header</span></span>|<span data-ttu-id="cb350-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cb350-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb350-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb350-122">Authorization</span></span>|<span data-ttu-id="cb350-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb350-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb350-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb350-124">Accept</span></span>|<span data-ttu-id="cb350-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb350-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb350-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb350-126">Request body</span></span>
<span data-ttu-id="cb350-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="cb350-127">In the request body, supply a JSON representation for the windowsMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="cb350-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="cb350-128">The following table shows the properties that are required when you create the windowsMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="cb350-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb350-129">Property</span></span>|<span data-ttu-id="cb350-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb350-130">Type</span></span>|<span data-ttu-id="cb350-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb350-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb350-132">id</span><span class="sxs-lookup"><span data-stu-id="cb350-132">id</span></span>|<span data-ttu-id="cb350-133">String</span><span class="sxs-lookup"><span data-stu-id="cb350-133">String</span></span>|<span data-ttu-id="cb350-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cb350-134">Key of the entity.</span></span> <span data-ttu-id="cb350-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cb350-136">displayName</span></span>|<span data-ttu-id="cb350-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb350-137">String</span></span>|<span data-ttu-id="cb350-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cb350-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cb350-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-140">descrição</span><span class="sxs-lookup"><span data-stu-id="cb350-140">description</span></span>|<span data-ttu-id="cb350-141">String</span><span class="sxs-lookup"><span data-stu-id="cb350-141">String</span></span>|<span data-ttu-id="cb350-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb350-142">The description of the app.</span></span> <span data-ttu-id="cb350-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-144">publicador</span><span class="sxs-lookup"><span data-stu-id="cb350-144">publisher</span></span>|<span data-ttu-id="cb350-145">String</span><span class="sxs-lookup"><span data-stu-id="cb350-145">String</span></span>|<span data-ttu-id="cb350-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb350-146">The publisher of the app.</span></span> <span data-ttu-id="cb350-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cb350-148">largeIcon</span></span>|[<span data-ttu-id="cb350-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cb350-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cb350-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="cb350-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cb350-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb350-152">createdDateTime</span></span>|<span data-ttu-id="cb350-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb350-153">DateTimeOffset</span></span>|<span data-ttu-id="cb350-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb350-154">The date and time the app was created.</span></span> <span data-ttu-id="cb350-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb350-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cb350-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb350-157">DateTimeOffset</span></span>|<span data-ttu-id="cb350-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cb350-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cb350-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cb350-160">isFeatured</span></span>|<span data-ttu-id="cb350-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb350-161">Boolean</span></span>|<span data-ttu-id="cb350-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cb350-163">privacyInformationUrl</span></span>|<span data-ttu-id="cb350-164">String</span><span class="sxs-lookup"><span data-stu-id="cb350-164">String</span></span>|<span data-ttu-id="cb350-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cb350-165">The privacy statement Url.</span></span> <span data-ttu-id="cb350-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cb350-167">informationUrl</span></span>|<span data-ttu-id="cb350-168">String</span><span class="sxs-lookup"><span data-stu-id="cb350-168">String</span></span>|<span data-ttu-id="cb350-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cb350-169">The more information Url.</span></span> <span data-ttu-id="cb350-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-171">owner</span><span class="sxs-lookup"><span data-stu-id="cb350-171">owner</span></span>|<span data-ttu-id="cb350-172">String</span><span class="sxs-lookup"><span data-stu-id="cb350-172">String</span></span>|<span data-ttu-id="cb350-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cb350-173">The owner of the app.</span></span> <span data-ttu-id="cb350-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-175">developer</span><span class="sxs-lookup"><span data-stu-id="cb350-175">developer</span></span>|<span data-ttu-id="cb350-176">String</span><span class="sxs-lookup"><span data-stu-id="cb350-176">String</span></span>|<span data-ttu-id="cb350-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb350-177">The developer of the app.</span></span> <span data-ttu-id="cb350-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-179">notes</span><span class="sxs-lookup"><span data-stu-id="cb350-179">notes</span></span>|<span data-ttu-id="cb350-180">String</span><span class="sxs-lookup"><span data-stu-id="cb350-180">String</span></span>|<span data-ttu-id="cb350-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb350-181">Notes for the app.</span></span> <span data-ttu-id="cb350-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cb350-183">uploadState</span></span>|<span data-ttu-id="cb350-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cb350-184">Int32</span></span>|<span data-ttu-id="cb350-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="cb350-185">The upload state.</span></span> <span data-ttu-id="cb350-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cb350-187">publishingState</span></span>|[<span data-ttu-id="cb350-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cb350-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cb350-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cb350-189">The publishing state for the app.</span></span> <span data-ttu-id="cb350-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="cb350-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cb350-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb350-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="cb350-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cb350-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cb350-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cb350-193">isAssigned</span></span>|<span data-ttu-id="cb350-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb350-194">Boolean</span></span>|<span data-ttu-id="cb350-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="cb350-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cb350-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb350-197">roleScopeTagIds</span></span>|<span data-ttu-id="cb350-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb350-198">String collection</span></span>|<span data-ttu-id="cb350-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="cb350-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cb350-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="cb350-201">dependentAppCount</span></span>|<span data-ttu-id="cb350-202">Int32</span><span class="sxs-lookup"><span data-stu-id="cb350-202">Int32</span></span>|<span data-ttu-id="cb350-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="cb350-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="cb350-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb350-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cb350-205">canal</span><span class="sxs-lookup"><span data-stu-id="cb350-205">channel</span></span>|[<span data-ttu-id="cb350-206">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="cb350-206">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="cb350-207">O canal a ser instalado nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="cb350-207">The channel to install on target devices.</span></span> <span data-ttu-id="cb350-208">Os valores possíveis são: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="cb350-208">Possible values are: `dev`, `beta`, `stable`.</span></span>|
|<span data-ttu-id="cb350-209">displayLanguageLocale</span><span class="sxs-lookup"><span data-stu-id="cb350-209">displayLanguageLocale</span></span>|<span data-ttu-id="cb350-210">String</span><span class="sxs-lookup"><span data-stu-id="cb350-210">String</span></span>|<span data-ttu-id="cb350-211">A localidade do idioma a ser usada quando o aplicativo de borda exibe texto para o usuário.</span><span class="sxs-lookup"><span data-stu-id="cb350-211">The language locale to use when the Edge app displays text to the user.</span></span>|



## <a name="response"></a><span data-ttu-id="cb350-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb350-212">Response</span></span>
<span data-ttu-id="cb350-213">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb350-213">If successful, this method returns a `201 Created` response code and a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb350-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb350-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb350-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb350-215">Request</span></span>
<span data-ttu-id="cb350-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb350-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cb350-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb350-217">Response</span></span>
<span data-ttu-id="cb350-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb350-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





