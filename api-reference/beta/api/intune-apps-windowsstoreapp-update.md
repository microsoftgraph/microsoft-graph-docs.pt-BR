---
title: Atualizar windowsStoreApp
description: Atualiza as propriedades de um objeto windowsStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70af1c90ed719569181d33d1566e8aa0f16e76a7
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791873"
---
# <a name="update-windowsstoreapp"></a><span data-ttu-id="ee452-103">Atualizar windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="ee452-103">Update windowsStoreApp</span></span>

<span data-ttu-id="ee452-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee452-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee452-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee452-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee452-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee452-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee452-107">Atualiza as propriedades de um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ee452-107">Update the properties of a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee452-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee452-108">Prerequisites</span></span>
<span data-ttu-id="ee452-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee452-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee452-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee452-111">Permission type</span></span>|<span data-ttu-id="ee452-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee452-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee452-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee452-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee452-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee452-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ee452-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee452-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee452-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee452-116">Not supported.</span></span>|
|<span data-ttu-id="ee452-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee452-117">Application</span></span>|<span data-ttu-id="ee452-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee452-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee452-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee452-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ee452-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee452-120">Request headers</span></span>
|<span data-ttu-id="ee452-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee452-121">Header</span></span>|<span data-ttu-id="ee452-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee452-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee452-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee452-123">Authorization</span></span>|<span data-ttu-id="ee452-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee452-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee452-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee452-125">Accept</span></span>|<span data-ttu-id="ee452-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee452-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee452-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee452-127">Request body</span></span>
<span data-ttu-id="ee452-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ee452-128">In the request body, supply a JSON representation for the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

<span data-ttu-id="ee452-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee452-129">The following table shows the properties that are required when you create the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

|<span data-ttu-id="ee452-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee452-130">Property</span></span>|<span data-ttu-id="ee452-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee452-131">Type</span></span>|<span data-ttu-id="ee452-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee452-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee452-133">id</span><span class="sxs-lookup"><span data-stu-id="ee452-133">id</span></span>|<span data-ttu-id="ee452-134">String</span><span class="sxs-lookup"><span data-stu-id="ee452-134">String</span></span>|<span data-ttu-id="ee452-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ee452-135">Key of the entity.</span></span> <span data-ttu-id="ee452-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ee452-137">displayName</span></span>|<span data-ttu-id="ee452-138">String</span><span class="sxs-lookup"><span data-stu-id="ee452-138">String</span></span>|<span data-ttu-id="ee452-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ee452-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ee452-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-141">description</span><span class="sxs-lookup"><span data-stu-id="ee452-141">description</span></span>|<span data-ttu-id="ee452-142">String</span><span class="sxs-lookup"><span data-stu-id="ee452-142">String</span></span>|<span data-ttu-id="ee452-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee452-143">The description of the app.</span></span> <span data-ttu-id="ee452-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-145">publicador</span><span class="sxs-lookup"><span data-stu-id="ee452-145">publisher</span></span>|<span data-ttu-id="ee452-146">String</span><span class="sxs-lookup"><span data-stu-id="ee452-146">String</span></span>|<span data-ttu-id="ee452-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee452-147">The publisher of the app.</span></span> <span data-ttu-id="ee452-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ee452-149">largeIcon</span></span>|[<span data-ttu-id="ee452-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ee452-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ee452-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ee452-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ee452-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee452-153">createdDateTime</span></span>|<span data-ttu-id="ee452-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee452-154">DateTimeOffset</span></span>|<span data-ttu-id="ee452-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee452-155">The date and time the app was created.</span></span> <span data-ttu-id="ee452-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee452-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ee452-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee452-158">DateTimeOffset</span></span>|<span data-ttu-id="ee452-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ee452-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ee452-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ee452-161">isFeatured</span></span>|<span data-ttu-id="ee452-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee452-162">Boolean</span></span>|<span data-ttu-id="ee452-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ee452-164">privacyInformationUrl</span></span>|<span data-ttu-id="ee452-165">String</span><span class="sxs-lookup"><span data-stu-id="ee452-165">String</span></span>|<span data-ttu-id="ee452-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ee452-166">The privacy statement Url.</span></span> <span data-ttu-id="ee452-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ee452-168">informationUrl</span></span>|<span data-ttu-id="ee452-169">String</span><span class="sxs-lookup"><span data-stu-id="ee452-169">String</span></span>|<span data-ttu-id="ee452-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ee452-170">The more information Url.</span></span> <span data-ttu-id="ee452-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-172">owner</span><span class="sxs-lookup"><span data-stu-id="ee452-172">owner</span></span>|<span data-ttu-id="ee452-173">String</span><span class="sxs-lookup"><span data-stu-id="ee452-173">String</span></span>|<span data-ttu-id="ee452-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ee452-174">The owner of the app.</span></span> <span data-ttu-id="ee452-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-176">developer</span><span class="sxs-lookup"><span data-stu-id="ee452-176">developer</span></span>|<span data-ttu-id="ee452-177">String</span><span class="sxs-lookup"><span data-stu-id="ee452-177">String</span></span>|<span data-ttu-id="ee452-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee452-178">The developer of the app.</span></span> <span data-ttu-id="ee452-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-180">notes</span><span class="sxs-lookup"><span data-stu-id="ee452-180">notes</span></span>|<span data-ttu-id="ee452-181">String</span><span class="sxs-lookup"><span data-stu-id="ee452-181">String</span></span>|<span data-ttu-id="ee452-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee452-182">Notes for the app.</span></span> <span data-ttu-id="ee452-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ee452-184">uploadState</span></span>|<span data-ttu-id="ee452-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ee452-185">Int32</span></span>|<span data-ttu-id="ee452-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="ee452-186">The upload state.</span></span> <span data-ttu-id="ee452-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ee452-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ee452-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ee452-189">publishingState</span></span>|[<span data-ttu-id="ee452-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ee452-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ee452-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee452-191">The publishing state for the app.</span></span> <span data-ttu-id="ee452-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ee452-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ee452-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ee452-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ee452-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ee452-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ee452-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ee452-195">isAssigned</span></span>|<span data-ttu-id="ee452-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee452-196">Boolean</span></span>|<span data-ttu-id="ee452-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ee452-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ee452-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee452-199">roleScopeTagIds</span></span>|<span data-ttu-id="ee452-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee452-200">String collection</span></span>|<span data-ttu-id="ee452-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ee452-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ee452-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ee452-203">dependentAppCount</span></span>|<span data-ttu-id="ee452-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ee452-204">Int32</span></span>|<span data-ttu-id="ee452-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="ee452-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ee452-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ee452-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ee452-207">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ee452-207">appStoreUrl</span></span>|<span data-ttu-id="ee452-208">String</span><span class="sxs-lookup"><span data-stu-id="ee452-208">String</span></span>|<span data-ttu-id="ee452-209">A URL da loja de aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="ee452-209">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="ee452-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee452-210">Response</span></span>
<span data-ttu-id="ee452-211">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee452-211">If successful, this method returns a `200 OK` response code and an updated [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee452-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee452-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee452-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee452-213">Request</span></span>
<span data-ttu-id="ee452-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee452-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 768

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="ee452-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee452-215">Response</span></span>
<span data-ttu-id="ee452-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee452-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 940

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```



