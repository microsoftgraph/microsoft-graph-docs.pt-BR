---
title: Criar macOSMdatpApp
description: Criar um novo objeto macOSMdatpApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d972a78219f0fefee6a3e5c9502ee8d1b9a8d41c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445383"
---
# <a name="create-macosmdatpapp"></a><span data-ttu-id="17424-103">Criar macOSMdatpApp</span><span class="sxs-lookup"><span data-stu-id="17424-103">Create macOSMdatpApp</span></span>

<span data-ttu-id="17424-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="17424-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17424-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17424-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17424-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17424-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17424-107">Criar um novo objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="17424-107">Create a new [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17424-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17424-108">Prerequisites</span></span>
<span data-ttu-id="17424-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17424-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17424-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17424-111">Permission type</span></span>|<span data-ttu-id="17424-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17424-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17424-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17424-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17424-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17424-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17424-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17424-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17424-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17424-116">Not supported.</span></span>|
|<span data-ttu-id="17424-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17424-117">Application</span></span>|<span data-ttu-id="17424-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17424-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17424-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17424-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="17424-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17424-120">Request headers</span></span>
|<span data-ttu-id="17424-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17424-121">Header</span></span>|<span data-ttu-id="17424-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17424-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17424-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17424-123">Authorization</span></span>|<span data-ttu-id="17424-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17424-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17424-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17424-125">Accept</span></span>|<span data-ttu-id="17424-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17424-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17424-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17424-127">Request body</span></span>
<span data-ttu-id="17424-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSMdatpApp.</span><span class="sxs-lookup"><span data-stu-id="17424-128">In the request body, supply a JSON representation for the macOSMdatpApp object.</span></span>

<span data-ttu-id="17424-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSMdatpApp.</span><span class="sxs-lookup"><span data-stu-id="17424-129">The following table shows the properties that are required when you create the macOSMdatpApp.</span></span>

|<span data-ttu-id="17424-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17424-130">Property</span></span>|<span data-ttu-id="17424-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17424-131">Type</span></span>|<span data-ttu-id="17424-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17424-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17424-133">id</span><span class="sxs-lookup"><span data-stu-id="17424-133">id</span></span>|<span data-ttu-id="17424-134">String</span><span class="sxs-lookup"><span data-stu-id="17424-134">String</span></span>|<span data-ttu-id="17424-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="17424-135">Key of the entity.</span></span> <span data-ttu-id="17424-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-137">displayName</span><span class="sxs-lookup"><span data-stu-id="17424-137">displayName</span></span>|<span data-ttu-id="17424-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17424-138">String</span></span>|<span data-ttu-id="17424-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="17424-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="17424-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-141">description</span><span class="sxs-lookup"><span data-stu-id="17424-141">description</span></span>|<span data-ttu-id="17424-142">String</span><span class="sxs-lookup"><span data-stu-id="17424-142">String</span></span>|<span data-ttu-id="17424-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17424-143">The description of the app.</span></span> <span data-ttu-id="17424-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-145">publicador</span><span class="sxs-lookup"><span data-stu-id="17424-145">publisher</span></span>|<span data-ttu-id="17424-146">String</span><span class="sxs-lookup"><span data-stu-id="17424-146">String</span></span>|<span data-ttu-id="17424-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17424-147">The publisher of the app.</span></span> <span data-ttu-id="17424-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="17424-149">largeIcon</span></span>|[<span data-ttu-id="17424-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="17424-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="17424-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="17424-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="17424-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17424-153">createdDateTime</span></span>|<span data-ttu-id="17424-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17424-154">DateTimeOffset</span></span>|<span data-ttu-id="17424-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17424-155">The date and time the app was created.</span></span> <span data-ttu-id="17424-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17424-157">lastModifiedDateTime</span></span>|<span data-ttu-id="17424-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17424-158">DateTimeOffset</span></span>|<span data-ttu-id="17424-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="17424-159">The date and time the app was last modified.</span></span> <span data-ttu-id="17424-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="17424-161">isFeatured</span></span>|<span data-ttu-id="17424-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="17424-162">Boolean</span></span>|<span data-ttu-id="17424-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="17424-164">privacyInformationUrl</span></span>|<span data-ttu-id="17424-165">String</span><span class="sxs-lookup"><span data-stu-id="17424-165">String</span></span>|<span data-ttu-id="17424-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="17424-166">The privacy statement Url.</span></span> <span data-ttu-id="17424-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="17424-168">informationUrl</span></span>|<span data-ttu-id="17424-169">String</span><span class="sxs-lookup"><span data-stu-id="17424-169">String</span></span>|<span data-ttu-id="17424-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="17424-170">The more information Url.</span></span> <span data-ttu-id="17424-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-172">owner</span><span class="sxs-lookup"><span data-stu-id="17424-172">owner</span></span>|<span data-ttu-id="17424-173">String</span><span class="sxs-lookup"><span data-stu-id="17424-173">String</span></span>|<span data-ttu-id="17424-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="17424-174">The owner of the app.</span></span> <span data-ttu-id="17424-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-176">developer</span><span class="sxs-lookup"><span data-stu-id="17424-176">developer</span></span>|<span data-ttu-id="17424-177">String</span><span class="sxs-lookup"><span data-stu-id="17424-177">String</span></span>|<span data-ttu-id="17424-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17424-178">The developer of the app.</span></span> <span data-ttu-id="17424-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-180">notes</span><span class="sxs-lookup"><span data-stu-id="17424-180">notes</span></span>|<span data-ttu-id="17424-181">String</span><span class="sxs-lookup"><span data-stu-id="17424-181">String</span></span>|<span data-ttu-id="17424-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17424-182">Notes for the app.</span></span> <span data-ttu-id="17424-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="17424-184">uploadState</span></span>|<span data-ttu-id="17424-185">Int32</span><span class="sxs-lookup"><span data-stu-id="17424-185">Int32</span></span>|<span data-ttu-id="17424-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="17424-186">The upload state.</span></span> <span data-ttu-id="17424-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="17424-188">publishingState</span></span>|[<span data-ttu-id="17424-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="17424-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="17424-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17424-190">The publishing state for the app.</span></span> <span data-ttu-id="17424-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="17424-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="17424-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17424-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="17424-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="17424-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="17424-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="17424-194">isAssigned</span></span>|<span data-ttu-id="17424-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="17424-195">Boolean</span></span>|<span data-ttu-id="17424-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="17424-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="17424-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17424-198">roleScopeTagIds</span></span>|<span data-ttu-id="17424-199">String collection</span><span class="sxs-lookup"><span data-stu-id="17424-199">String collection</span></span>|<span data-ttu-id="17424-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="17424-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="17424-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17424-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="17424-202">dependentAppCount</span></span>|<span data-ttu-id="17424-203">Int32</span><span class="sxs-lookup"><span data-stu-id="17424-203">Int32</span></span>|<span data-ttu-id="17424-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="17424-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="17424-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17424-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="17424-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="17424-206">Response</span></span>
<span data-ttu-id="17424-207">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17424-207">If successful, this method returns a `201 Created` response code and a [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17424-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17424-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="17424-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17424-209">Request</span></span>
<span data-ttu-id="17424-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17424-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 712

{
  "@odata.type": "#microsoft.graph.macOSMdatpApp",
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

### <a name="response"></a><span data-ttu-id="17424-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="17424-211">Response</span></span>
<span data-ttu-id="17424-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17424-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 884

{
  "@odata.type": "#microsoft.graph.macOSMdatpApp",
  "id": "2963b007-b007-2963-07b0-632907b06329",
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





