---
title: Criar macOSOfficeSuiteApp
description: Criar um novo objeto macOSOfficeSuiteApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9a6ed23c52b79576cfe4063e4495da4b8b058dd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935899"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="819c5-103">Criar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="819c5-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="819c5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="819c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="819c5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="819c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="819c5-106">Criar um novo objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="819c5-106">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="819c5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="819c5-107">Prerequisites</span></span>
<span data-ttu-id="819c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="819c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="819c5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="819c5-110">Permission type</span></span>|<span data-ttu-id="819c5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="819c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="819c5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="819c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="819c5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="819c5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="819c5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="819c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="819c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="819c5-115">Not supported.</span></span>|
|<span data-ttu-id="819c5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="819c5-116">Application</span></span>|<span data-ttu-id="819c5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="819c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="819c5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="819c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="819c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="819c5-119">Request headers</span></span>
|<span data-ttu-id="819c5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="819c5-120">Header</span></span>|<span data-ttu-id="819c5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="819c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="819c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="819c5-122">Authorization</span></span>|<span data-ttu-id="819c5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="819c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="819c5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="819c5-124">Accept</span></span>|<span data-ttu-id="819c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="819c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="819c5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="819c5-126">Request body</span></span>
<span data-ttu-id="819c5-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="819c5-127">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="819c5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="819c5-128">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="819c5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="819c5-129">Property</span></span>|<span data-ttu-id="819c5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="819c5-130">Type</span></span>|<span data-ttu-id="819c5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="819c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="819c5-132">id</span><span class="sxs-lookup"><span data-stu-id="819c5-132">id</span></span>|<span data-ttu-id="819c5-133">String</span><span class="sxs-lookup"><span data-stu-id="819c5-133">String</span></span>|<span data-ttu-id="819c5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="819c5-134">Key of the entity.</span></span> <span data-ttu-id="819c5-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="819c5-136">displayName</span></span>|<span data-ttu-id="819c5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="819c5-137">String</span></span>|<span data-ttu-id="819c5-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="819c5-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="819c5-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-140">description</span><span class="sxs-lookup"><span data-stu-id="819c5-140">description</span></span>|<span data-ttu-id="819c5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="819c5-141">String</span></span>|<span data-ttu-id="819c5-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="819c5-142">The description of the app.</span></span> <span data-ttu-id="819c5-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-144">publicador</span><span class="sxs-lookup"><span data-stu-id="819c5-144">publisher</span></span>|<span data-ttu-id="819c5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="819c5-145">String</span></span>|<span data-ttu-id="819c5-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="819c5-146">The publisher of the app.</span></span> <span data-ttu-id="819c5-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="819c5-148">largeIcon</span></span>|[<span data-ttu-id="819c5-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="819c5-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="819c5-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="819c5-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="819c5-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="819c5-152">createdDateTime</span></span>|<span data-ttu-id="819c5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="819c5-153">DateTimeOffset</span></span>|<span data-ttu-id="819c5-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="819c5-154">The date and time the app was created.</span></span> <span data-ttu-id="819c5-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="819c5-156">lastModifiedDateTime</span></span>|<span data-ttu-id="819c5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="819c5-157">DateTimeOffset</span></span>|<span data-ttu-id="819c5-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="819c5-158">The date and time the app was last modified.</span></span> <span data-ttu-id="819c5-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="819c5-160">isFeatured</span></span>|<span data-ttu-id="819c5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="819c5-161">Boolean</span></span>|<span data-ttu-id="819c5-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="819c5-163">privacyInformationUrl</span></span>|<span data-ttu-id="819c5-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="819c5-164">String</span></span>|<span data-ttu-id="819c5-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="819c5-165">The privacy statement Url.</span></span> <span data-ttu-id="819c5-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="819c5-167">informationUrl</span></span>|<span data-ttu-id="819c5-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="819c5-168">String</span></span>|<span data-ttu-id="819c5-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="819c5-169">The more information Url.</span></span> <span data-ttu-id="819c5-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-171">owner</span><span class="sxs-lookup"><span data-stu-id="819c5-171">owner</span></span>|<span data-ttu-id="819c5-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="819c5-172">String</span></span>|<span data-ttu-id="819c5-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="819c5-173">The owner of the app.</span></span> <span data-ttu-id="819c5-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-175">developer</span><span class="sxs-lookup"><span data-stu-id="819c5-175">developer</span></span>|<span data-ttu-id="819c5-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="819c5-176">String</span></span>|<span data-ttu-id="819c5-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="819c5-177">The developer of the app.</span></span> <span data-ttu-id="819c5-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-179">notes</span><span class="sxs-lookup"><span data-stu-id="819c5-179">notes</span></span>|<span data-ttu-id="819c5-180">String</span><span class="sxs-lookup"><span data-stu-id="819c5-180">String</span></span>|<span data-ttu-id="819c5-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="819c5-181">Notes for the app.</span></span> <span data-ttu-id="819c5-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="819c5-183">uploadState</span></span>|<span data-ttu-id="819c5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="819c5-184">Int32</span></span>|<span data-ttu-id="819c5-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="819c5-185">The upload state.</span></span> <span data-ttu-id="819c5-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="819c5-187">publishingState</span></span>|[<span data-ttu-id="819c5-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="819c5-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="819c5-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="819c5-189">The publishing state for the app.</span></span> <span data-ttu-id="819c5-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="819c5-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="819c5-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="819c5-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="819c5-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="819c5-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="819c5-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="819c5-193">isAssigned</span></span>|<span data-ttu-id="819c5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="819c5-194">Boolean</span></span>|<span data-ttu-id="819c5-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="819c5-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="819c5-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="819c5-197">roleScopeTagIds</span></span>|<span data-ttu-id="819c5-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="819c5-198">String collection</span></span>|<span data-ttu-id="819c5-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="819c5-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="819c5-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="819c5-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="819c5-201">dependentAppCount</span></span>|<span data-ttu-id="819c5-202">Int32</span><span class="sxs-lookup"><span data-stu-id="819c5-202">Int32</span></span>|<span data-ttu-id="819c5-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="819c5-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="819c5-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="819c5-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="819c5-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="819c5-205">Response</span></span>
<span data-ttu-id="819c5-206">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="819c5-206">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="819c5-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="819c5-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="819c5-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="819c5-208">Request</span></span>
<span data-ttu-id="819c5-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="819c5-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 718

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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

### <a name="response"></a><span data-ttu-id="819c5-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="819c5-210">Response</span></span>
<span data-ttu-id="819c5-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="819c5-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 890

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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




