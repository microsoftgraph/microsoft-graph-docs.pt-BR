---
title: Criar macOSOfficeSuiteApp
description: Criar um novo objeto macOSOfficeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1286fc93b684410dec49741d75c47b0b245c3e8
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792048"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="97fb6-103">Criar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="97fb6-103">Create macOSOfficeSuiteApp</span></span>

<span data-ttu-id="97fb6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97fb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97fb6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97fb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97fb6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97fb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97fb6-107">Criar um novo objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="97fb6-107">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97fb6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97fb6-108">Prerequisites</span></span>
<span data-ttu-id="97fb6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97fb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97fb6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97fb6-111">Permission type</span></span>|<span data-ttu-id="97fb6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97fb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97fb6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97fb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97fb6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97fb6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="97fb6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97fb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97fb6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97fb6-116">Not supported.</span></span>|
|<span data-ttu-id="97fb6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97fb6-117">Application</span></span>|<span data-ttu-id="97fb6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97fb6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97fb6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97fb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="97fb6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97fb6-120">Request headers</span></span>
|<span data-ttu-id="97fb6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97fb6-121">Header</span></span>|<span data-ttu-id="97fb6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97fb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97fb6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97fb6-123">Authorization</span></span>|<span data-ttu-id="97fb6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97fb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97fb6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97fb6-125">Accept</span></span>|<span data-ttu-id="97fb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97fb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97fb6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97fb6-127">Request body</span></span>
<span data-ttu-id="97fb6-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="97fb6-128">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="97fb6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="97fb6-129">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="97fb6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97fb6-130">Property</span></span>|<span data-ttu-id="97fb6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97fb6-131">Type</span></span>|<span data-ttu-id="97fb6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97fb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97fb6-133">id</span><span class="sxs-lookup"><span data-stu-id="97fb6-133">id</span></span>|<span data-ttu-id="97fb6-134">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-134">String</span></span>|<span data-ttu-id="97fb6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="97fb6-135">Key of the entity.</span></span> <span data-ttu-id="97fb6-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="97fb6-137">displayName</span></span>|<span data-ttu-id="97fb6-138">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-138">String</span></span>|<span data-ttu-id="97fb6-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="97fb6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="97fb6-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-141">description</span><span class="sxs-lookup"><span data-stu-id="97fb6-141">description</span></span>|<span data-ttu-id="97fb6-142">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-142">String</span></span>|<span data-ttu-id="97fb6-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97fb6-143">The description of the app.</span></span> <span data-ttu-id="97fb6-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-145">publicador</span><span class="sxs-lookup"><span data-stu-id="97fb6-145">publisher</span></span>|<span data-ttu-id="97fb6-146">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-146">String</span></span>|<span data-ttu-id="97fb6-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97fb6-147">The publisher of the app.</span></span> <span data-ttu-id="97fb6-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="97fb6-149">largeIcon</span></span>|[<span data-ttu-id="97fb6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="97fb6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="97fb6-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="97fb6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="97fb6-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97fb6-153">createdDateTime</span></span>|<span data-ttu-id="97fb6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97fb6-154">DateTimeOffset</span></span>|<span data-ttu-id="97fb6-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97fb6-155">The date and time the app was created.</span></span> <span data-ttu-id="97fb6-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97fb6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="97fb6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97fb6-158">DateTimeOffset</span></span>|<span data-ttu-id="97fb6-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="97fb6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="97fb6-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="97fb6-161">isFeatured</span></span>|<span data-ttu-id="97fb6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="97fb6-162">Boolean</span></span>|<span data-ttu-id="97fb6-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="97fb6-164">privacyInformationUrl</span></span>|<span data-ttu-id="97fb6-165">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-165">String</span></span>|<span data-ttu-id="97fb6-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="97fb6-166">The privacy statement Url.</span></span> <span data-ttu-id="97fb6-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="97fb6-168">informationUrl</span></span>|<span data-ttu-id="97fb6-169">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-169">String</span></span>|<span data-ttu-id="97fb6-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="97fb6-170">The more information Url.</span></span> <span data-ttu-id="97fb6-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-172">owner</span><span class="sxs-lookup"><span data-stu-id="97fb6-172">owner</span></span>|<span data-ttu-id="97fb6-173">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-173">String</span></span>|<span data-ttu-id="97fb6-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="97fb6-174">The owner of the app.</span></span> <span data-ttu-id="97fb6-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-176">developer</span><span class="sxs-lookup"><span data-stu-id="97fb6-176">developer</span></span>|<span data-ttu-id="97fb6-177">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-177">String</span></span>|<span data-ttu-id="97fb6-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97fb6-178">The developer of the app.</span></span> <span data-ttu-id="97fb6-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-180">notes</span><span class="sxs-lookup"><span data-stu-id="97fb6-180">notes</span></span>|<span data-ttu-id="97fb6-181">String</span><span class="sxs-lookup"><span data-stu-id="97fb6-181">String</span></span>|<span data-ttu-id="97fb6-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97fb6-182">Notes for the app.</span></span> <span data-ttu-id="97fb6-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="97fb6-184">uploadState</span></span>|<span data-ttu-id="97fb6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="97fb6-185">Int32</span></span>|<span data-ttu-id="97fb6-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="97fb6-186">The upload state.</span></span> <span data-ttu-id="97fb6-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="97fb6-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="97fb6-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="97fb6-189">publishingState</span></span>|[<span data-ttu-id="97fb6-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="97fb6-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="97fb6-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97fb6-191">The publishing state for the app.</span></span> <span data-ttu-id="97fb6-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="97fb6-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="97fb6-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="97fb6-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="97fb6-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="97fb6-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="97fb6-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="97fb6-195">isAssigned</span></span>|<span data-ttu-id="97fb6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="97fb6-196">Boolean</span></span>|<span data-ttu-id="97fb6-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="97fb6-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="97fb6-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97fb6-199">roleScopeTagIds</span></span>|<span data-ttu-id="97fb6-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97fb6-200">String collection</span></span>|<span data-ttu-id="97fb6-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="97fb6-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="97fb6-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="97fb6-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="97fb6-203">dependentAppCount</span></span>|<span data-ttu-id="97fb6-204">Int32</span><span class="sxs-lookup"><span data-stu-id="97fb6-204">Int32</span></span>|<span data-ttu-id="97fb6-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="97fb6-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="97fb6-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="97fb6-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="97fb6-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="97fb6-207">Response</span></span>
<span data-ttu-id="97fb6-208">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97fb6-208">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97fb6-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97fb6-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="97fb6-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97fb6-210">Request</span></span>
<span data-ttu-id="97fb6-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97fb6-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97fb6-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="97fb6-212">Response</span></span>
<span data-ttu-id="97fb6-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97fb6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



