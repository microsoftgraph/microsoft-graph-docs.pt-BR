---
title: Criar macOSMicrosoftEdgeApp
description: Criar um novo objeto macOSMicrosoftEdgeApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8687bba8a99017caa4af727f47fe7a929932f4e6
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535342"
---
# <a name="create-macosmicrosoftedgeapp"></a><span data-ttu-id="475d7-103">Criar macOSMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="475d7-103">Create macOSMicrosoftEdgeApp</span></span>

> <span data-ttu-id="475d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="475d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="475d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="475d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="475d7-106">Criar um novo objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="475d7-106">Create a new [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="475d7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="475d7-107">Prerequisites</span></span>
<span data-ttu-id="475d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="475d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="475d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="475d7-110">Permission type</span></span>|<span data-ttu-id="475d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="475d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="475d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="475d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="475d7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475d7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="475d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="475d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="475d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="475d7-115">Not supported.</span></span>|
|<span data-ttu-id="475d7-116">Application</span><span class="sxs-lookup"><span data-stu-id="475d7-116">Application</span></span>|<span data-ttu-id="475d7-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475d7-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="475d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="475d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="475d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="475d7-119">Request headers</span></span>
|<span data-ttu-id="475d7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="475d7-120">Header</span></span>|<span data-ttu-id="475d7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="475d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="475d7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="475d7-122">Authorization</span></span>|<span data-ttu-id="475d7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="475d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="475d7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="475d7-124">Accept</span></span>|<span data-ttu-id="475d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="475d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="475d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="475d7-126">Request body</span></span>
<span data-ttu-id="475d7-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="475d7-127">In the request body, supply a JSON representation for the macOSMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="475d7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="475d7-128">The following table shows the properties that are required when you create the macOSMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="475d7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="475d7-129">Property</span></span>|<span data-ttu-id="475d7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="475d7-130">Type</span></span>|<span data-ttu-id="475d7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="475d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="475d7-132">id</span><span class="sxs-lookup"><span data-stu-id="475d7-132">id</span></span>|<span data-ttu-id="475d7-133">String</span><span class="sxs-lookup"><span data-stu-id="475d7-133">String</span></span>|<span data-ttu-id="475d7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="475d7-134">Key of the entity.</span></span> <span data-ttu-id="475d7-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="475d7-136">displayName</span></span>|<span data-ttu-id="475d7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475d7-137">String</span></span>|<span data-ttu-id="475d7-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="475d7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="475d7-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-140">description</span><span class="sxs-lookup"><span data-stu-id="475d7-140">description</span></span>|<span data-ttu-id="475d7-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475d7-141">String</span></span>|<span data-ttu-id="475d7-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="475d7-142">The description of the app.</span></span> <span data-ttu-id="475d7-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-144">publicador</span><span class="sxs-lookup"><span data-stu-id="475d7-144">publisher</span></span>|<span data-ttu-id="475d7-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475d7-145">String</span></span>|<span data-ttu-id="475d7-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="475d7-146">The publisher of the app.</span></span> <span data-ttu-id="475d7-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="475d7-148">largeIcon</span></span>|[<span data-ttu-id="475d7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="475d7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="475d7-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="475d7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="475d7-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="475d7-152">createdDateTime</span></span>|<span data-ttu-id="475d7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="475d7-153">DateTimeOffset</span></span>|<span data-ttu-id="475d7-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="475d7-154">The date and time the app was created.</span></span> <span data-ttu-id="475d7-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="475d7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="475d7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="475d7-157">DateTimeOffset</span></span>|<span data-ttu-id="475d7-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="475d7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="475d7-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="475d7-160">isFeatured</span></span>|<span data-ttu-id="475d7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="475d7-161">Boolean</span></span>|<span data-ttu-id="475d7-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="475d7-163">privacyInformationUrl</span></span>|<span data-ttu-id="475d7-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475d7-164">String</span></span>|<span data-ttu-id="475d7-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="475d7-165">The privacy statement Url.</span></span> <span data-ttu-id="475d7-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="475d7-167">informationUrl</span></span>|<span data-ttu-id="475d7-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475d7-168">String</span></span>|<span data-ttu-id="475d7-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="475d7-169">The more information Url.</span></span> <span data-ttu-id="475d7-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-171">owner</span><span class="sxs-lookup"><span data-stu-id="475d7-171">owner</span></span>|<span data-ttu-id="475d7-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475d7-172">String</span></span>|<span data-ttu-id="475d7-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="475d7-173">The owner of the app.</span></span> <span data-ttu-id="475d7-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-175">developer</span><span class="sxs-lookup"><span data-stu-id="475d7-175">developer</span></span>|<span data-ttu-id="475d7-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="475d7-176">String</span></span>|<span data-ttu-id="475d7-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="475d7-177">The developer of the app.</span></span> <span data-ttu-id="475d7-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-179">notes</span><span class="sxs-lookup"><span data-stu-id="475d7-179">notes</span></span>|<span data-ttu-id="475d7-180">String</span><span class="sxs-lookup"><span data-stu-id="475d7-180">String</span></span>|<span data-ttu-id="475d7-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="475d7-181">Notes for the app.</span></span> <span data-ttu-id="475d7-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="475d7-183">uploadState</span></span>|<span data-ttu-id="475d7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="475d7-184">Int32</span></span>|<span data-ttu-id="475d7-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="475d7-185">The upload state.</span></span> <span data-ttu-id="475d7-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="475d7-187">publishingState</span></span>|[<span data-ttu-id="475d7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="475d7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="475d7-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="475d7-189">The publishing state for the app.</span></span> <span data-ttu-id="475d7-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="475d7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="475d7-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="475d7-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="475d7-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="475d7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="475d7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="475d7-193">isAssigned</span></span>|<span data-ttu-id="475d7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="475d7-194">Boolean</span></span>|<span data-ttu-id="475d7-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="475d7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="475d7-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="475d7-197">roleScopeTagIds</span></span>|<span data-ttu-id="475d7-198">String collection</span><span class="sxs-lookup"><span data-stu-id="475d7-198">String collection</span></span>|<span data-ttu-id="475d7-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="475d7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="475d7-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="475d7-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="475d7-201">dependentAppCount</span></span>|<span data-ttu-id="475d7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="475d7-202">Int32</span></span>|<span data-ttu-id="475d7-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="475d7-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="475d7-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="475d7-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="475d7-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="475d7-205">Response</span></span>
<span data-ttu-id="475d7-206">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="475d7-206">If successful, this method returns a `201 Created` response code and a [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="475d7-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="475d7-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="475d7-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="475d7-208">Request</span></span>
<span data-ttu-id="475d7-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="475d7-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 720

{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
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
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="475d7-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="475d7-210">Response</span></span>
<span data-ttu-id="475d7-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="475d7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 892

{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
  "id": "c964092a-092a-c964-2a09-64c92a0964c9",
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
  "dependentAppCount": 1
}
```






