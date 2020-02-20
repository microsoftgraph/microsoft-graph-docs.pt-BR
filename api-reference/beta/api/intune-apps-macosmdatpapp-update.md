---
title: Atualizar macOSMdatpApp
description: Atualiza as propriedades de um objeto macOSMdatpApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3aebf41624512975b44a6f551f54bac6f9556c3f
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160789"
---
# <a name="update-macosmdatpapp"></a><span data-ttu-id="49bba-103">Atualizar macOSMdatpApp</span><span class="sxs-lookup"><span data-stu-id="49bba-103">Update macOSMdatpApp</span></span>

> <span data-ttu-id="49bba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49bba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49bba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49bba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49bba-106">Atualiza as propriedades de um objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="49bba-106">Update the properties of a [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49bba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49bba-107">Prerequisites</span></span>
<span data-ttu-id="49bba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49bba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49bba-110">Permission type</span></span>|<span data-ttu-id="49bba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49bba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49bba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49bba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49bba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49bba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="49bba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49bba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49bba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49bba-115">Not supported.</span></span>|
|<span data-ttu-id="49bba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49bba-116">Application</span></span>|<span data-ttu-id="49bba-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49bba-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49bba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49bba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="49bba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49bba-119">Request headers</span></span>
|<span data-ttu-id="49bba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49bba-120">Header</span></span>|<span data-ttu-id="49bba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49bba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49bba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49bba-122">Authorization</span></span>|<span data-ttu-id="49bba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49bba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49bba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49bba-124">Accept</span></span>|<span data-ttu-id="49bba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49bba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49bba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49bba-126">Request body</span></span>
<span data-ttu-id="49bba-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="49bba-127">In the request body, supply a JSON representation for the [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

<span data-ttu-id="49bba-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md).</span><span class="sxs-lookup"><span data-stu-id="49bba-128">The following table shows the properties that are required when you create the [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md).</span></span>

|<span data-ttu-id="49bba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49bba-129">Property</span></span>|<span data-ttu-id="49bba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="49bba-130">Type</span></span>|<span data-ttu-id="49bba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="49bba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49bba-132">id</span><span class="sxs-lookup"><span data-stu-id="49bba-132">id</span></span>|<span data-ttu-id="49bba-133">String</span><span class="sxs-lookup"><span data-stu-id="49bba-133">String</span></span>|<span data-ttu-id="49bba-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="49bba-134">Key of the entity.</span></span> <span data-ttu-id="49bba-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="49bba-136">displayName</span></span>|<span data-ttu-id="49bba-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49bba-137">String</span></span>|<span data-ttu-id="49bba-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="49bba-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="49bba-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-140">descrição</span><span class="sxs-lookup"><span data-stu-id="49bba-140">description</span></span>|<span data-ttu-id="49bba-141">String</span><span class="sxs-lookup"><span data-stu-id="49bba-141">String</span></span>|<span data-ttu-id="49bba-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bba-142">The description of the app.</span></span> <span data-ttu-id="49bba-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-144">publicador</span><span class="sxs-lookup"><span data-stu-id="49bba-144">publisher</span></span>|<span data-ttu-id="49bba-145">String</span><span class="sxs-lookup"><span data-stu-id="49bba-145">String</span></span>|<span data-ttu-id="49bba-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bba-146">The publisher of the app.</span></span> <span data-ttu-id="49bba-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="49bba-148">largeIcon</span></span>|[<span data-ttu-id="49bba-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="49bba-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="49bba-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="49bba-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="49bba-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49bba-152">createdDateTime</span></span>|<span data-ttu-id="49bba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49bba-153">DateTimeOffset</span></span>|<span data-ttu-id="49bba-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bba-154">The date and time the app was created.</span></span> <span data-ttu-id="49bba-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49bba-156">lastModifiedDateTime</span></span>|<span data-ttu-id="49bba-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49bba-157">DateTimeOffset</span></span>|<span data-ttu-id="49bba-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="49bba-158">The date and time the app was last modified.</span></span> <span data-ttu-id="49bba-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="49bba-160">isFeatured</span></span>|<span data-ttu-id="49bba-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="49bba-161">Boolean</span></span>|<span data-ttu-id="49bba-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="49bba-163">privacyInformationUrl</span></span>|<span data-ttu-id="49bba-164">String</span><span class="sxs-lookup"><span data-stu-id="49bba-164">String</span></span>|<span data-ttu-id="49bba-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="49bba-165">The privacy statement Url.</span></span> <span data-ttu-id="49bba-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="49bba-167">informationUrl</span></span>|<span data-ttu-id="49bba-168">String</span><span class="sxs-lookup"><span data-stu-id="49bba-168">String</span></span>|<span data-ttu-id="49bba-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="49bba-169">The more information Url.</span></span> <span data-ttu-id="49bba-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-171">owner</span><span class="sxs-lookup"><span data-stu-id="49bba-171">owner</span></span>|<span data-ttu-id="49bba-172">String</span><span class="sxs-lookup"><span data-stu-id="49bba-172">String</span></span>|<span data-ttu-id="49bba-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="49bba-173">The owner of the app.</span></span> <span data-ttu-id="49bba-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-175">developer</span><span class="sxs-lookup"><span data-stu-id="49bba-175">developer</span></span>|<span data-ttu-id="49bba-176">String</span><span class="sxs-lookup"><span data-stu-id="49bba-176">String</span></span>|<span data-ttu-id="49bba-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bba-177">The developer of the app.</span></span> <span data-ttu-id="49bba-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-179">notes</span><span class="sxs-lookup"><span data-stu-id="49bba-179">notes</span></span>|<span data-ttu-id="49bba-180">String</span><span class="sxs-lookup"><span data-stu-id="49bba-180">String</span></span>|<span data-ttu-id="49bba-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bba-181">Notes for the app.</span></span> <span data-ttu-id="49bba-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="49bba-183">uploadState</span></span>|<span data-ttu-id="49bba-184">Int32</span><span class="sxs-lookup"><span data-stu-id="49bba-184">Int32</span></span>|<span data-ttu-id="49bba-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="49bba-185">The upload state.</span></span> <span data-ttu-id="49bba-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="49bba-187">publishingState</span></span>|[<span data-ttu-id="49bba-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="49bba-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="49bba-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bba-189">The publishing state for the app.</span></span> <span data-ttu-id="49bba-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="49bba-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="49bba-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49bba-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="49bba-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="49bba-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="49bba-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="49bba-193">isAssigned</span></span>|<span data-ttu-id="49bba-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="49bba-194">Boolean</span></span>|<span data-ttu-id="49bba-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="49bba-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="49bba-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49bba-197">roleScopeTagIds</span></span>|<span data-ttu-id="49bba-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="49bba-198">String collection</span></span>|<span data-ttu-id="49bba-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="49bba-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="49bba-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bba-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="49bba-201">dependentAppCount</span></span>|<span data-ttu-id="49bba-202">Int32</span><span class="sxs-lookup"><span data-stu-id="49bba-202">Int32</span></span>|<span data-ttu-id="49bba-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="49bba-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="49bba-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bba-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="49bba-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="49bba-205">Response</span></span>
<span data-ttu-id="49bba-206">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49bba-206">If successful, this method returns a `200 OK` response code and an updated [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49bba-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49bba-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="49bba-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49bba-208">Request</span></span>
<span data-ttu-id="49bba-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49bba-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="49bba-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="49bba-210">Response</span></span>
<span data-ttu-id="49bba-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49bba-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





