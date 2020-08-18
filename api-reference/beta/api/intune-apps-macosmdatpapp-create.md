---
title: Criar macOSMdatpApp
description: Criar um novo objeto macOSMdatpApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d35e57aea572ec1a603283b49210763a6b93ba6
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792090"
---
# <a name="create-macosmdatpapp"></a><span data-ttu-id="0fbea-103">Criar macOSMdatpApp</span><span class="sxs-lookup"><span data-stu-id="0fbea-103">Create macOSMdatpApp</span></span>

<span data-ttu-id="0fbea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fbea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fbea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0fbea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fbea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0fbea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fbea-107">Criar um novo objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="0fbea-107">Create a new [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fbea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fbea-108">Prerequisites</span></span>
<span data-ttu-id="0fbea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fbea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fbea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fbea-111">Permission type</span></span>|<span data-ttu-id="0fbea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0fbea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fbea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fbea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fbea-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fbea-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0fbea-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fbea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fbea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fbea-116">Not supported.</span></span>|
|<span data-ttu-id="0fbea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fbea-117">Application</span></span>|<span data-ttu-id="0fbea-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fbea-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fbea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fbea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0fbea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fbea-120">Request headers</span></span>
|<span data-ttu-id="0fbea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fbea-121">Header</span></span>|<span data-ttu-id="0fbea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0fbea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fbea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fbea-123">Authorization</span></span>|<span data-ttu-id="0fbea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fbea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fbea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fbea-125">Accept</span></span>|<span data-ttu-id="0fbea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fbea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fbea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fbea-127">Request body</span></span>
<span data-ttu-id="0fbea-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSMdatpApp.</span><span class="sxs-lookup"><span data-stu-id="0fbea-128">In the request body, supply a JSON representation for the macOSMdatpApp object.</span></span>

<span data-ttu-id="0fbea-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSMdatpApp.</span><span class="sxs-lookup"><span data-stu-id="0fbea-129">The following table shows the properties that are required when you create the macOSMdatpApp.</span></span>

|<span data-ttu-id="0fbea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fbea-130">Property</span></span>|<span data-ttu-id="0fbea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fbea-131">Type</span></span>|<span data-ttu-id="0fbea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fbea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fbea-133">id</span><span class="sxs-lookup"><span data-stu-id="0fbea-133">id</span></span>|<span data-ttu-id="0fbea-134">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-134">String</span></span>|<span data-ttu-id="0fbea-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0fbea-135">Key of the entity.</span></span> <span data-ttu-id="0fbea-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0fbea-137">displayName</span></span>|<span data-ttu-id="0fbea-138">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-138">String</span></span>|<span data-ttu-id="0fbea-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0fbea-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0fbea-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-141">description</span><span class="sxs-lookup"><span data-stu-id="0fbea-141">description</span></span>|<span data-ttu-id="0fbea-142">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-142">String</span></span>|<span data-ttu-id="0fbea-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0fbea-143">The description of the app.</span></span> <span data-ttu-id="0fbea-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-145">publicador</span><span class="sxs-lookup"><span data-stu-id="0fbea-145">publisher</span></span>|<span data-ttu-id="0fbea-146">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-146">String</span></span>|<span data-ttu-id="0fbea-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0fbea-147">The publisher of the app.</span></span> <span data-ttu-id="0fbea-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0fbea-149">largeIcon</span></span>|[<span data-ttu-id="0fbea-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0fbea-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0fbea-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0fbea-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0fbea-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fbea-153">createdDateTime</span></span>|<span data-ttu-id="0fbea-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fbea-154">DateTimeOffset</span></span>|<span data-ttu-id="0fbea-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0fbea-155">The date and time the app was created.</span></span> <span data-ttu-id="0fbea-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fbea-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0fbea-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fbea-158">DateTimeOffset</span></span>|<span data-ttu-id="0fbea-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0fbea-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0fbea-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0fbea-161">isFeatured</span></span>|<span data-ttu-id="0fbea-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fbea-162">Boolean</span></span>|<span data-ttu-id="0fbea-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0fbea-164">privacyInformationUrl</span></span>|<span data-ttu-id="0fbea-165">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-165">String</span></span>|<span data-ttu-id="0fbea-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0fbea-166">The privacy statement Url.</span></span> <span data-ttu-id="0fbea-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0fbea-168">informationUrl</span></span>|<span data-ttu-id="0fbea-169">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-169">String</span></span>|<span data-ttu-id="0fbea-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0fbea-170">The more information Url.</span></span> <span data-ttu-id="0fbea-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-172">owner</span><span class="sxs-lookup"><span data-stu-id="0fbea-172">owner</span></span>|<span data-ttu-id="0fbea-173">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-173">String</span></span>|<span data-ttu-id="0fbea-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0fbea-174">The owner of the app.</span></span> <span data-ttu-id="0fbea-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-176">developer</span><span class="sxs-lookup"><span data-stu-id="0fbea-176">developer</span></span>|<span data-ttu-id="0fbea-177">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-177">String</span></span>|<span data-ttu-id="0fbea-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0fbea-178">The developer of the app.</span></span> <span data-ttu-id="0fbea-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-180">notes</span><span class="sxs-lookup"><span data-stu-id="0fbea-180">notes</span></span>|<span data-ttu-id="0fbea-181">String</span><span class="sxs-lookup"><span data-stu-id="0fbea-181">String</span></span>|<span data-ttu-id="0fbea-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0fbea-182">Notes for the app.</span></span> <span data-ttu-id="0fbea-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0fbea-184">uploadState</span></span>|<span data-ttu-id="0fbea-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0fbea-185">Int32</span></span>|<span data-ttu-id="0fbea-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="0fbea-186">The upload state.</span></span> <span data-ttu-id="0fbea-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="0fbea-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="0fbea-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="0fbea-189">publishingState</span></span>|[<span data-ttu-id="0fbea-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0fbea-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0fbea-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0fbea-191">The publishing state for the app.</span></span> <span data-ttu-id="0fbea-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0fbea-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0fbea-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0fbea-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="0fbea-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0fbea-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0fbea-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0fbea-195">isAssigned</span></span>|<span data-ttu-id="0fbea-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fbea-196">Boolean</span></span>|<span data-ttu-id="0fbea-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="0fbea-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0fbea-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0fbea-199">roleScopeTagIds</span></span>|<span data-ttu-id="0fbea-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fbea-200">String collection</span></span>|<span data-ttu-id="0fbea-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0fbea-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0fbea-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0fbea-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0fbea-203">dependentAppCount</span></span>|<span data-ttu-id="0fbea-204">Int32</span><span class="sxs-lookup"><span data-stu-id="0fbea-204">Int32</span></span>|<span data-ttu-id="0fbea-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="0fbea-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0fbea-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fbea-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0fbea-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fbea-207">Response</span></span>
<span data-ttu-id="0fbea-208">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fbea-208">If successful, this method returns a `201 Created` response code and a [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fbea-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fbea-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fbea-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fbea-210">Request</span></span>
<span data-ttu-id="0fbea-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fbea-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0fbea-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fbea-212">Response</span></span>
<span data-ttu-id="0fbea-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fbea-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



