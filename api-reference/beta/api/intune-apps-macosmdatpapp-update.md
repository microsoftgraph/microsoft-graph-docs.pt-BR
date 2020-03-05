---
title: Atualizar macOSMdatpApp
description: Atualiza as propriedades de um objeto macOSMdatpApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e786d4f2a90dbea02ba78fc8583a7a672ac119cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445313"
---
# <a name="update-macosmdatpapp"></a><span data-ttu-id="8c861-103">Atualizar macOSMdatpApp</span><span class="sxs-lookup"><span data-stu-id="8c861-103">Update macOSMdatpApp</span></span>

<span data-ttu-id="8c861-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c861-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c861-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c861-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c861-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c861-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c861-107">Atualiza as propriedades de um objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8c861-107">Update the properties of a [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c861-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c861-108">Prerequisites</span></span>
<span data-ttu-id="8c861-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c861-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c861-111">Permission type</span></span>|<span data-ttu-id="8c861-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c861-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c861-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c861-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c861-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c861-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c861-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c861-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c861-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c861-116">Not supported.</span></span>|
|<span data-ttu-id="8c861-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c861-117">Application</span></span>|<span data-ttu-id="8c861-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c861-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c861-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c861-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8c861-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c861-120">Request headers</span></span>
|<span data-ttu-id="8c861-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c861-121">Header</span></span>|<span data-ttu-id="8c861-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c861-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c861-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c861-123">Authorization</span></span>|<span data-ttu-id="8c861-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c861-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c861-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c861-125">Accept</span></span>|<span data-ttu-id="8c861-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c861-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c861-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c861-127">Request body</span></span>
<span data-ttu-id="8c861-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8c861-128">In the request body, supply a JSON representation for the [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

<span data-ttu-id="8c861-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c861-129">The following table shows the properties that are required when you create the [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md).</span></span>

|<span data-ttu-id="8c861-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c861-130">Property</span></span>|<span data-ttu-id="8c861-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c861-131">Type</span></span>|<span data-ttu-id="8c861-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c861-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c861-133">id</span><span class="sxs-lookup"><span data-stu-id="8c861-133">id</span></span>|<span data-ttu-id="8c861-134">String</span><span class="sxs-lookup"><span data-stu-id="8c861-134">String</span></span>|<span data-ttu-id="8c861-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c861-135">Key of the entity.</span></span> <span data-ttu-id="8c861-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8c861-137">displayName</span></span>|<span data-ttu-id="8c861-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c861-138">String</span></span>|<span data-ttu-id="8c861-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8c861-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8c861-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-141">description</span><span class="sxs-lookup"><span data-stu-id="8c861-141">description</span></span>|<span data-ttu-id="8c861-142">String</span><span class="sxs-lookup"><span data-stu-id="8c861-142">String</span></span>|<span data-ttu-id="8c861-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c861-143">The description of the app.</span></span> <span data-ttu-id="8c861-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-145">publicador</span><span class="sxs-lookup"><span data-stu-id="8c861-145">publisher</span></span>|<span data-ttu-id="8c861-146">String</span><span class="sxs-lookup"><span data-stu-id="8c861-146">String</span></span>|<span data-ttu-id="8c861-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c861-147">The publisher of the app.</span></span> <span data-ttu-id="8c861-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8c861-149">largeIcon</span></span>|[<span data-ttu-id="8c861-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8c861-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8c861-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8c861-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8c861-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c861-153">createdDateTime</span></span>|<span data-ttu-id="8c861-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c861-154">DateTimeOffset</span></span>|<span data-ttu-id="8c861-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c861-155">The date and time the app was created.</span></span> <span data-ttu-id="8c861-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c861-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8c861-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c861-158">DateTimeOffset</span></span>|<span data-ttu-id="8c861-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8c861-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8c861-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8c861-161">isFeatured</span></span>|<span data-ttu-id="8c861-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c861-162">Boolean</span></span>|<span data-ttu-id="8c861-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8c861-164">privacyInformationUrl</span></span>|<span data-ttu-id="8c861-165">String</span><span class="sxs-lookup"><span data-stu-id="8c861-165">String</span></span>|<span data-ttu-id="8c861-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8c861-166">The privacy statement Url.</span></span> <span data-ttu-id="8c861-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8c861-168">informationUrl</span></span>|<span data-ttu-id="8c861-169">String</span><span class="sxs-lookup"><span data-stu-id="8c861-169">String</span></span>|<span data-ttu-id="8c861-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8c861-170">The more information Url.</span></span> <span data-ttu-id="8c861-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-172">owner</span><span class="sxs-lookup"><span data-stu-id="8c861-172">owner</span></span>|<span data-ttu-id="8c861-173">String</span><span class="sxs-lookup"><span data-stu-id="8c861-173">String</span></span>|<span data-ttu-id="8c861-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8c861-174">The owner of the app.</span></span> <span data-ttu-id="8c861-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-176">developer</span><span class="sxs-lookup"><span data-stu-id="8c861-176">developer</span></span>|<span data-ttu-id="8c861-177">String</span><span class="sxs-lookup"><span data-stu-id="8c861-177">String</span></span>|<span data-ttu-id="8c861-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c861-178">The developer of the app.</span></span> <span data-ttu-id="8c861-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-180">notes</span><span class="sxs-lookup"><span data-stu-id="8c861-180">notes</span></span>|<span data-ttu-id="8c861-181">String</span><span class="sxs-lookup"><span data-stu-id="8c861-181">String</span></span>|<span data-ttu-id="8c861-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c861-182">Notes for the app.</span></span> <span data-ttu-id="8c861-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8c861-184">uploadState</span></span>|<span data-ttu-id="8c861-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8c861-185">Int32</span></span>|<span data-ttu-id="8c861-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="8c861-186">The upload state.</span></span> <span data-ttu-id="8c861-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8c861-188">publishingState</span></span>|[<span data-ttu-id="8c861-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8c861-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8c861-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c861-190">The publishing state for the app.</span></span> <span data-ttu-id="8c861-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8c861-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8c861-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8c861-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8c861-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8c861-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8c861-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8c861-194">isAssigned</span></span>|<span data-ttu-id="8c861-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c861-195">Boolean</span></span>|<span data-ttu-id="8c861-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="8c861-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8c861-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8c861-198">roleScopeTagIds</span></span>|<span data-ttu-id="8c861-199">String collection</span><span class="sxs-lookup"><span data-stu-id="8c861-199">String collection</span></span>|<span data-ttu-id="8c861-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8c861-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8c861-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8c861-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8c861-202">dependentAppCount</span></span>|<span data-ttu-id="8c861-203">Int32</span><span class="sxs-lookup"><span data-stu-id="8c861-203">Int32</span></span>|<span data-ttu-id="8c861-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="8c861-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8c861-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c861-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8c861-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c861-206">Response</span></span>
<span data-ttu-id="8c861-207">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c861-207">If successful, this method returns a `200 OK` response code and an updated [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c861-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c861-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c861-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c861-209">Request</span></span>
<span data-ttu-id="8c861-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c861-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8c861-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c861-211">Response</span></span>
<span data-ttu-id="8c861-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c861-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





