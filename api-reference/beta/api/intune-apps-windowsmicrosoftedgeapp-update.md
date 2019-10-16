---
title: Atualizar windowsMicrosoftEdgeApp
description: Atualiza as propriedades de um objeto windowsMicrosoftEdgeApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9baeb98d146a2af412e94791f1eb9bb1847c3224
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535055"
---
# <a name="update-windowsmicrosoftedgeapp"></a><span data-ttu-id="446d4-103">Atualizar windowsMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="446d4-103">Update windowsMicrosoftEdgeApp</span></span>

> <span data-ttu-id="446d4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="446d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="446d4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="446d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="446d4-106">Atualiza as propriedades de um objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="446d4-106">Update the properties of a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="446d4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="446d4-107">Prerequisites</span></span>
<span data-ttu-id="446d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="446d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="446d4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="446d4-110">Permission type</span></span>|<span data-ttu-id="446d4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="446d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="446d4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="446d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="446d4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446d4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="446d4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="446d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="446d4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="446d4-115">Not supported.</span></span>|
|<span data-ttu-id="446d4-116">Application</span><span class="sxs-lookup"><span data-stu-id="446d4-116">Application</span></span>|<span data-ttu-id="446d4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446d4-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="446d4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="446d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="446d4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="446d4-119">Request headers</span></span>
|<span data-ttu-id="446d4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="446d4-120">Header</span></span>|<span data-ttu-id="446d4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="446d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="446d4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="446d4-122">Authorization</span></span>|<span data-ttu-id="446d4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="446d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="446d4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="446d4-124">Accept</span></span>|<span data-ttu-id="446d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="446d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="446d4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="446d4-126">Request body</span></span>
<span data-ttu-id="446d4-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="446d4-127">In the request body, supply a JSON representation for the [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

<span data-ttu-id="446d4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md).</span><span class="sxs-lookup"><span data-stu-id="446d4-128">The following table shows the properties that are required when you create the [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md).</span></span>

|<span data-ttu-id="446d4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="446d4-129">Property</span></span>|<span data-ttu-id="446d4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="446d4-130">Type</span></span>|<span data-ttu-id="446d4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="446d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="446d4-132">id</span><span class="sxs-lookup"><span data-stu-id="446d4-132">id</span></span>|<span data-ttu-id="446d4-133">String</span><span class="sxs-lookup"><span data-stu-id="446d4-133">String</span></span>|<span data-ttu-id="446d4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="446d4-134">Key of the entity.</span></span> <span data-ttu-id="446d4-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="446d4-136">displayName</span></span>|<span data-ttu-id="446d4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d4-137">String</span></span>|<span data-ttu-id="446d4-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="446d4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="446d4-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-140">description</span><span class="sxs-lookup"><span data-stu-id="446d4-140">description</span></span>|<span data-ttu-id="446d4-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d4-141">String</span></span>|<span data-ttu-id="446d4-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="446d4-142">The description of the app.</span></span> <span data-ttu-id="446d4-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-144">publicador</span><span class="sxs-lookup"><span data-stu-id="446d4-144">publisher</span></span>|<span data-ttu-id="446d4-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d4-145">String</span></span>|<span data-ttu-id="446d4-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="446d4-146">The publisher of the app.</span></span> <span data-ttu-id="446d4-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="446d4-148">largeIcon</span></span>|[<span data-ttu-id="446d4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="446d4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="446d4-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="446d4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="446d4-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="446d4-152">createdDateTime</span></span>|<span data-ttu-id="446d4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="446d4-153">DateTimeOffset</span></span>|<span data-ttu-id="446d4-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="446d4-154">The date and time the app was created.</span></span> <span data-ttu-id="446d4-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="446d4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="446d4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="446d4-157">DateTimeOffset</span></span>|<span data-ttu-id="446d4-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="446d4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="446d4-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="446d4-160">isFeatured</span></span>|<span data-ttu-id="446d4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="446d4-161">Boolean</span></span>|<span data-ttu-id="446d4-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="446d4-163">privacyInformationUrl</span></span>|<span data-ttu-id="446d4-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d4-164">String</span></span>|<span data-ttu-id="446d4-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="446d4-165">The privacy statement Url.</span></span> <span data-ttu-id="446d4-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="446d4-167">informationUrl</span></span>|<span data-ttu-id="446d4-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d4-168">String</span></span>|<span data-ttu-id="446d4-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="446d4-169">The more information Url.</span></span> <span data-ttu-id="446d4-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-171">owner</span><span class="sxs-lookup"><span data-stu-id="446d4-171">owner</span></span>|<span data-ttu-id="446d4-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d4-172">String</span></span>|<span data-ttu-id="446d4-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="446d4-173">The owner of the app.</span></span> <span data-ttu-id="446d4-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-175">developer</span><span class="sxs-lookup"><span data-stu-id="446d4-175">developer</span></span>|<span data-ttu-id="446d4-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="446d4-176">String</span></span>|<span data-ttu-id="446d4-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="446d4-177">The developer of the app.</span></span> <span data-ttu-id="446d4-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-179">notes</span><span class="sxs-lookup"><span data-stu-id="446d4-179">notes</span></span>|<span data-ttu-id="446d4-180">String</span><span class="sxs-lookup"><span data-stu-id="446d4-180">String</span></span>|<span data-ttu-id="446d4-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="446d4-181">Notes for the app.</span></span> <span data-ttu-id="446d4-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="446d4-183">uploadState</span></span>|<span data-ttu-id="446d4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="446d4-184">Int32</span></span>|<span data-ttu-id="446d4-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="446d4-185">The upload state.</span></span> <span data-ttu-id="446d4-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="446d4-187">publishingState</span></span>|[<span data-ttu-id="446d4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="446d4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="446d4-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="446d4-189">The publishing state for the app.</span></span> <span data-ttu-id="446d4-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="446d4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="446d4-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="446d4-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="446d4-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="446d4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="446d4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="446d4-193">isAssigned</span></span>|<span data-ttu-id="446d4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="446d4-194">Boolean</span></span>|<span data-ttu-id="446d4-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="446d4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="446d4-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="446d4-197">roleScopeTagIds</span></span>|<span data-ttu-id="446d4-198">String collection</span><span class="sxs-lookup"><span data-stu-id="446d4-198">String collection</span></span>|<span data-ttu-id="446d4-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="446d4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="446d4-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="446d4-201">dependentAppCount</span></span>|<span data-ttu-id="446d4-202">Int32</span><span class="sxs-lookup"><span data-stu-id="446d4-202">Int32</span></span>|<span data-ttu-id="446d4-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="446d4-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="446d4-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="446d4-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="446d4-205">canal</span><span class="sxs-lookup"><span data-stu-id="446d4-205">channel</span></span>|[<span data-ttu-id="446d4-206">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="446d4-206">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="446d4-207">O canal a ser instalado nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="446d4-207">The channel to install on target devices.</span></span> <span data-ttu-id="446d4-208">Os valores possíveis são: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="446d4-208">Possible values are: `dev`, `beta`, `stable`.</span></span>|



## <a name="response"></a><span data-ttu-id="446d4-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="446d4-209">Response</span></span>
<span data-ttu-id="446d4-210">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="446d4-210">If successful, this method returns a `200 OK` response code and an updated [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="446d4-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="446d4-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="446d4-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="446d4-212">Request</span></span>
<span data-ttu-id="446d4-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="446d4-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 744

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
  "channel": "beta"
}
```

### <a name="response"></a><span data-ttu-id="446d4-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="446d4-214">Response</span></span>
<span data-ttu-id="446d4-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="446d4-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 916

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
  "channel": "beta"
}
```






