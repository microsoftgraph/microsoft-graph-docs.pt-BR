---
title: Atualizar windowsPhone81StoreApp
description: Atualiza as propriedades de um objeto windowsPhone81StoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86da2a11f81e59c8a5860a10df08004af1d2d7f8
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790053"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="7a370-103">Atualizar windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="7a370-103">Update windowsPhone81StoreApp</span></span>

<span data-ttu-id="7a370-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a370-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a370-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a370-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a370-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a370-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a370-107">Atualiza as propriedades de um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7a370-107">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a370-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a370-108">Prerequisites</span></span>
<span data-ttu-id="7a370-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a370-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a370-111">Permission type</span></span>|<span data-ttu-id="7a370-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a370-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a370-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a370-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a370-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a370-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7a370-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a370-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a370-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a370-116">Not supported.</span></span>|
|<span data-ttu-id="7a370-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a370-117">Application</span></span>|<span data-ttu-id="7a370-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a370-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a370-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a370-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7a370-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a370-120">Request headers</span></span>
|<span data-ttu-id="7a370-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a370-121">Header</span></span>|<span data-ttu-id="7a370-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7a370-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a370-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a370-123">Authorization</span></span>|<span data-ttu-id="7a370-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a370-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a370-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a370-125">Accept</span></span>|<span data-ttu-id="7a370-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a370-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a370-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a370-127">Request body</span></span>
<span data-ttu-id="7a370-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7a370-128">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="7a370-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a370-129">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="7a370-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a370-130">Property</span></span>|<span data-ttu-id="7a370-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a370-131">Type</span></span>|<span data-ttu-id="7a370-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a370-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a370-133">id</span><span class="sxs-lookup"><span data-stu-id="7a370-133">id</span></span>|<span data-ttu-id="7a370-134">String</span><span class="sxs-lookup"><span data-stu-id="7a370-134">String</span></span>|<span data-ttu-id="7a370-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7a370-135">Key of the entity.</span></span> <span data-ttu-id="7a370-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7a370-137">displayName</span></span>|<span data-ttu-id="7a370-138">String</span><span class="sxs-lookup"><span data-stu-id="7a370-138">String</span></span>|<span data-ttu-id="7a370-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7a370-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7a370-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-141">description</span><span class="sxs-lookup"><span data-stu-id="7a370-141">description</span></span>|<span data-ttu-id="7a370-142">String</span><span class="sxs-lookup"><span data-stu-id="7a370-142">String</span></span>|<span data-ttu-id="7a370-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a370-143">The description of the app.</span></span> <span data-ttu-id="7a370-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-145">publicador</span><span class="sxs-lookup"><span data-stu-id="7a370-145">publisher</span></span>|<span data-ttu-id="7a370-146">String</span><span class="sxs-lookup"><span data-stu-id="7a370-146">String</span></span>|<span data-ttu-id="7a370-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a370-147">The publisher of the app.</span></span> <span data-ttu-id="7a370-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7a370-149">largeIcon</span></span>|[<span data-ttu-id="7a370-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7a370-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7a370-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="7a370-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7a370-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a370-153">createdDateTime</span></span>|<span data-ttu-id="7a370-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a370-154">DateTimeOffset</span></span>|<span data-ttu-id="7a370-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a370-155">The date and time the app was created.</span></span> <span data-ttu-id="7a370-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a370-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7a370-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a370-158">DateTimeOffset</span></span>|<span data-ttu-id="7a370-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7a370-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7a370-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7a370-161">isFeatured</span></span>|<span data-ttu-id="7a370-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a370-162">Boolean</span></span>|<span data-ttu-id="7a370-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7a370-164">privacyInformationUrl</span></span>|<span data-ttu-id="7a370-165">String</span><span class="sxs-lookup"><span data-stu-id="7a370-165">String</span></span>|<span data-ttu-id="7a370-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7a370-166">The privacy statement Url.</span></span> <span data-ttu-id="7a370-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7a370-168">informationUrl</span></span>|<span data-ttu-id="7a370-169">String</span><span class="sxs-lookup"><span data-stu-id="7a370-169">String</span></span>|<span data-ttu-id="7a370-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="7a370-170">The more information Url.</span></span> <span data-ttu-id="7a370-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-172">owner</span><span class="sxs-lookup"><span data-stu-id="7a370-172">owner</span></span>|<span data-ttu-id="7a370-173">String</span><span class="sxs-lookup"><span data-stu-id="7a370-173">String</span></span>|<span data-ttu-id="7a370-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7a370-174">The owner of the app.</span></span> <span data-ttu-id="7a370-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-176">developer</span><span class="sxs-lookup"><span data-stu-id="7a370-176">developer</span></span>|<span data-ttu-id="7a370-177">String</span><span class="sxs-lookup"><span data-stu-id="7a370-177">String</span></span>|<span data-ttu-id="7a370-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a370-178">The developer of the app.</span></span> <span data-ttu-id="7a370-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-180">notes</span><span class="sxs-lookup"><span data-stu-id="7a370-180">notes</span></span>|<span data-ttu-id="7a370-181">String</span><span class="sxs-lookup"><span data-stu-id="7a370-181">String</span></span>|<span data-ttu-id="7a370-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a370-182">Notes for the app.</span></span> <span data-ttu-id="7a370-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7a370-184">uploadState</span></span>|<span data-ttu-id="7a370-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7a370-185">Int32</span></span>|<span data-ttu-id="7a370-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="7a370-186">The upload state.</span></span> <span data-ttu-id="7a370-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="7a370-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="7a370-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="7a370-189">publishingState</span></span>|[<span data-ttu-id="7a370-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7a370-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7a370-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a370-191">The publishing state for the app.</span></span> <span data-ttu-id="7a370-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="7a370-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7a370-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a370-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7a370-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7a370-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7a370-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7a370-195">isAssigned</span></span>|<span data-ttu-id="7a370-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a370-196">Boolean</span></span>|<span data-ttu-id="7a370-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="7a370-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7a370-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7a370-199">roleScopeTagIds</span></span>|<span data-ttu-id="7a370-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a370-200">String collection</span></span>|<span data-ttu-id="7a370-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="7a370-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7a370-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7a370-203">dependentAppCount</span></span>|<span data-ttu-id="7a370-204">Int32</span><span class="sxs-lookup"><span data-stu-id="7a370-204">Int32</span></span>|<span data-ttu-id="7a370-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="7a370-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7a370-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7a370-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7a370-207">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7a370-207">appStoreUrl</span></span>|<span data-ttu-id="7a370-208">String</span><span class="sxs-lookup"><span data-stu-id="7a370-208">String</span></span>|<span data-ttu-id="7a370-209">A URL da loja de aplicativos do Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="7a370-209">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="7a370-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a370-210">Response</span></span>
<span data-ttu-id="7a370-211">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a370-211">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a370-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a370-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a370-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a370-213">Request</span></span>
<span data-ttu-id="7a370-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a370-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 775

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
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

### <a name="response"></a><span data-ttu-id="7a370-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a370-215">Response</span></span>
<span data-ttu-id="7a370-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a370-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 947

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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



