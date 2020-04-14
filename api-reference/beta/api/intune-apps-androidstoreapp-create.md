---
title: Criar androidStoreApp
description: Criar um novo objeto androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ad7da84a59c5992c3b1f92d71e8394da901752e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417264"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="df369-103">Criar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="df369-103">Create androidStoreApp</span></span>

<span data-ttu-id="df369-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df369-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df369-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df369-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df369-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df369-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df369-107">Criar um novo objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="df369-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df369-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df369-108">Prerequisites</span></span>
<span data-ttu-id="df369-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df369-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df369-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df369-111">Permission type</span></span>|<span data-ttu-id="df369-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df369-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df369-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df369-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df369-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df369-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df369-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df369-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df369-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df369-116">Not supported.</span></span>|
|<span data-ttu-id="df369-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df369-117">Application</span></span>|<span data-ttu-id="df369-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df369-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df369-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df369-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="df369-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df369-120">Request headers</span></span>
|<span data-ttu-id="df369-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df369-121">Header</span></span>|<span data-ttu-id="df369-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df369-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df369-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df369-123">Authorization</span></span>|<span data-ttu-id="df369-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df369-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df369-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df369-125">Accept</span></span>|<span data-ttu-id="df369-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df369-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df369-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df369-127">Request body</span></span>
<span data-ttu-id="df369-128">No corpo da solicitação, forneça uma representação JSON do objeto androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="df369-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="df369-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="df369-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="df369-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df369-130">Property</span></span>|<span data-ttu-id="df369-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df369-131">Type</span></span>|<span data-ttu-id="df369-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df369-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df369-133">id</span><span class="sxs-lookup"><span data-stu-id="df369-133">id</span></span>|<span data-ttu-id="df369-134">String</span><span class="sxs-lookup"><span data-stu-id="df369-134">String</span></span>|<span data-ttu-id="df369-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="df369-135">Key of the entity.</span></span> <span data-ttu-id="df369-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-137">displayName</span><span class="sxs-lookup"><span data-stu-id="df369-137">displayName</span></span>|<span data-ttu-id="df369-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df369-138">String</span></span>|<span data-ttu-id="df369-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="df369-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="df369-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-141">description</span><span class="sxs-lookup"><span data-stu-id="df369-141">description</span></span>|<span data-ttu-id="df369-142">String</span><span class="sxs-lookup"><span data-stu-id="df369-142">String</span></span>|<span data-ttu-id="df369-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df369-143">The description of the app.</span></span> <span data-ttu-id="df369-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-145">publicador</span><span class="sxs-lookup"><span data-stu-id="df369-145">publisher</span></span>|<span data-ttu-id="df369-146">String</span><span class="sxs-lookup"><span data-stu-id="df369-146">String</span></span>|<span data-ttu-id="df369-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df369-147">The publisher of the app.</span></span> <span data-ttu-id="df369-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="df369-149">largeIcon</span></span>|[<span data-ttu-id="df369-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df369-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df369-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="df369-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="df369-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df369-153">createdDateTime</span></span>|<span data-ttu-id="df369-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df369-154">DateTimeOffset</span></span>|<span data-ttu-id="df369-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df369-155">The date and time the app was created.</span></span> <span data-ttu-id="df369-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df369-157">lastModifiedDateTime</span></span>|<span data-ttu-id="df369-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df369-158">DateTimeOffset</span></span>|<span data-ttu-id="df369-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="df369-159">The date and time the app was last modified.</span></span> <span data-ttu-id="df369-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="df369-161">isFeatured</span></span>|<span data-ttu-id="df369-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="df369-162">Boolean</span></span>|<span data-ttu-id="df369-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="df369-164">privacyInformationUrl</span></span>|<span data-ttu-id="df369-165">String</span><span class="sxs-lookup"><span data-stu-id="df369-165">String</span></span>|<span data-ttu-id="df369-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="df369-166">The privacy statement Url.</span></span> <span data-ttu-id="df369-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="df369-168">informationUrl</span></span>|<span data-ttu-id="df369-169">String</span><span class="sxs-lookup"><span data-stu-id="df369-169">String</span></span>|<span data-ttu-id="df369-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="df369-170">The more information Url.</span></span> <span data-ttu-id="df369-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-172">owner</span><span class="sxs-lookup"><span data-stu-id="df369-172">owner</span></span>|<span data-ttu-id="df369-173">String</span><span class="sxs-lookup"><span data-stu-id="df369-173">String</span></span>|<span data-ttu-id="df369-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="df369-174">The owner of the app.</span></span> <span data-ttu-id="df369-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-176">developer</span><span class="sxs-lookup"><span data-stu-id="df369-176">developer</span></span>|<span data-ttu-id="df369-177">String</span><span class="sxs-lookup"><span data-stu-id="df369-177">String</span></span>|<span data-ttu-id="df369-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df369-178">The developer of the app.</span></span> <span data-ttu-id="df369-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-180">notes</span><span class="sxs-lookup"><span data-stu-id="df369-180">notes</span></span>|<span data-ttu-id="df369-181">String</span><span class="sxs-lookup"><span data-stu-id="df369-181">String</span></span>|<span data-ttu-id="df369-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df369-182">Notes for the app.</span></span> <span data-ttu-id="df369-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="df369-184">uploadState</span></span>|<span data-ttu-id="df369-185">Int32</span><span class="sxs-lookup"><span data-stu-id="df369-185">Int32</span></span>|<span data-ttu-id="df369-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="df369-186">The upload state.</span></span> <span data-ttu-id="df369-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="df369-188">publishingState</span></span>|[<span data-ttu-id="df369-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="df369-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="df369-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df369-190">The publishing state for the app.</span></span> <span data-ttu-id="df369-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="df369-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="df369-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="df369-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="df369-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="df369-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="df369-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="df369-194">isAssigned</span></span>|<span data-ttu-id="df369-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="df369-195">Boolean</span></span>|<span data-ttu-id="df369-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="df369-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="df369-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df369-198">roleScopeTagIds</span></span>|<span data-ttu-id="df369-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="df369-199">String collection</span></span>|<span data-ttu-id="df369-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="df369-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="df369-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="df369-202">dependentAppCount</span></span>|<span data-ttu-id="df369-203">Int32</span><span class="sxs-lookup"><span data-stu-id="df369-203">Int32</span></span>|<span data-ttu-id="df369-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="df369-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="df369-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df369-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="df369-206">packageId</span><span class="sxs-lookup"><span data-stu-id="df369-206">packageId</span></span>|<span data-ttu-id="df369-207">String</span><span class="sxs-lookup"><span data-stu-id="df369-207">String</span></span>|<span data-ttu-id="df369-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="df369-208">The package identifier.</span></span>|
|<span data-ttu-id="df369-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="df369-209">appIdentifier</span></span>|<span data-ttu-id="df369-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df369-210">String</span></span>|<span data-ttu-id="df369-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="df369-211">The Identity Name.</span></span>|
|<span data-ttu-id="df369-212">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="df369-212">appStoreUrl</span></span>|<span data-ttu-id="df369-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df369-213">String</span></span>|<span data-ttu-id="df369-214">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="df369-214">The Android app store URL.</span></span>|
|<span data-ttu-id="df369-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="df369-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="df369-216">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="df369-216">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="df369-217">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="df369-217">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="df369-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="df369-218">Response</span></span>
<span data-ttu-id="df369-219">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df369-219">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df369-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df369-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="df369-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df369-221">Request</span></span>
<span data-ttu-id="df369-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df369-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1230

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="df369-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="df369-223">Response</span></span>
<span data-ttu-id="df369-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df369-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1402

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```



